0   ATXProdJournalTools�tg5    c  EcoResProductMasterDimTools�tg5c  �  ATXProdTableProdCut�tg5G    ATXGenerateProductPreProdTask�tg5T  �  ATXRequestOrderUpload�tg5�	  �  BOMCreate_Extension�tg5�  �  ATXRequestOrderNewVersion�tg5�  z   &EcoResProductMasterDimension_Extension�tg5  !  ATXRequestOrderAuthorize�tg50  C  ATXProdRouteMultiRegisterProd�tg5s   �  ATXRequestOrderUpdateCustRef�tg57  �  ATXRequestOrder�tg5�8  D  ATXInventJournalMuilti�tg5�@  I  ATXSalesBOMUpdate�tg55B  �   ATXFormCanvasLog�tg5�B  �  ATXTools�tg5`E  	  ATXApproveTasks�tg5iR  �   ATXProdCutPatternQtyUpdate�tg5S  :  ATXRouteCardContract�tg5KU    ATXReleaseBOMVersionVariants�tg5XW    ATXBOMMatrixEngine�tg5_[  p  ATXRouteCardController�tg5�f  �   ATXBOMVersionEngine�tg5�g  �	  ATXBOMTemplateEngine�tg5�q  �  ATXAXRequestOrderHeader�tg5<x  #	  ATXRequestOrderCreate�tg5_�  J  ATXPmfFormCtrl_BOMTemplateEdit�tg5��  c  ATXRequestOrderCopy�tg5�  �  ATXBreakdownOrderEngine�tg5Ֆ  '  ATXSalesLine_Extension�tg5��  ~  SalesTable_Extension�tg5z�  �  BOMCreateDialog_Extension�tg5I�  ,  ATXInventDimCtrl_Frm_ProductDim�tg5u�  �  ATXRequestOrderCancel�tg5f�  �  ATXLookupTableEngine�tg5�  �  %ATXProdJournalCheckPostProd_Extension�tg5��  �  ATXRequestBOMGenerateBatch�tg5s�  �  ATXUnApproveTasks�tg5]�  �   ATXProductTools�tg5	�  A  ATXReqTransPOMarkFirm_Extension�tg5J�  ~  (ATXWrkCtrResourceGroupCalendar_Extension�tg5ȳ  �  ATXProdJournalMulti�tg5e�  �  ATXBOMVersionVariants�tg5��  I  ATXBOMVersion_Extension�tg5D�  =  ATXRouteCardDP�tg5��  k  InventDimParm_Extension�tg5��  H  ATXItemGridEngine�tg54�  �  ATXInventMovement�tg5��  q  � ! 8class ATXProdJournalTools extends ATXFormCanvasLog
{
}ATXFormCanvasLog   � 
newProdJournalTable   � _prodId ProdId�� _prodJournalType ProdJournalType�� _description Description��  ProdJournalTable� �� 
postProdJournalBOMBF   � _prodJournalTable ProdJournalTable��  boolean� �ATXProdJournalTools�� ! )class EcoResProductMasterDimTools
{
}
   � 	
insertIfNotExistSize   � name EcoResSizeName��  � �� 	
insertIfNotExistColor   � name EcoResColorName��  � �� 	
insertIfNotExistConfiguration   � name EcoResConfigurationName��  � �� 	
%existEcoResProductMasterConfiguration   � productMaster RefRecId�� ConfigurationRecId EcoResConfigurationRecId�� hecoResProductDimensionAttribute::inventDimFieldId2DimensionAttributeRecId(fieldNum(InventDim, configId))dimensionAttributeRecId RefRecId��  boolean� �� 	
existEcoResProductMasterSize   � productMaster RefRecId�� 	sizeRecId EcoResSizeRecId�� lecoResProductDimensionAttribute::inventDimFieldId2DimensionAttributeRecId(fieldNum(InventDim, InventSizeId))dimensionAttributeRecId RefRecId��  boolean� �� 	
existEcoResProductMasterColor   � productMaster RefRecId�� 
ColorRecId EcoResColorRecId�� mecoResProductDimensionAttribute::inventDimFieldId2DimensionAttributeRecId(fieldNum(InventDim, InventColorId))dimensionAttributeRecId RefRecId��  boolean� �� 	
insertIfNotExistStyle   � name EcoResStyleName��  � �� 	
existEcoResProductMasterStyle   � productMaster RefRecId�� 
StyleRecId EcoResStyleRecId�� hecoResProductDimensionAttribute::inventDimFieldId2DimensionAttributeRecId(fieldNum(InventDim, configId))dimensionAttributeRecId RefRecId��  boolean� �EcoResProductMasterDimTools�� ! Bclass ATXProdTableProdCut
{
    ProdTable        prodTable;

}   " 	prodTable 	ProdTable�   � 
createFromProdTable   � 
_prodTable 	ProdTable��  � �� 
new   � 
_prodTable 	ProdTable��  � �� 
run�  � �ATXProdTableProdCut�� ! Zclass ATXGenerateProductPreProdTask
{
    ATXRequestOrderHeader requestOrderHeader;

}   " requestOrderHeader ATXRequestOrderHeader�   � 	
main   � _args Args��  � �� 
run�  ��� 
parmRequestOrderHeader   � _requestOrderHeader ATXRequestOrderHeader��  ATXRequestOrderHeader� �� 
generateTasksFromNewRequest�  ��ATXGenerateProductPreProdTask�� ! �/// <summary>
/// Create new versions and update version in RequestOrderHeader
/// </summary>
class ATXRequestOrderUpload extends FormRun
{
    Dialog                          dialog;
    DialogField                     dialogOption, dialogFileOpen, fieldApp;
    private str                     availableTypes = '.csv';
    private const str               okButtonName = 'OkButton';
    const str                       fileUploadName = 'FileUpload';
    const Delimiter                 delimiter = '\n';

    str                             textFile;
    str                             text;
    LineNumber                      lineNumber;
    Caption                         captionGroup;

    // Error log
    RecordInsertList                recordInsertListErrors;

    // Data
    ATXRequestOrderType        requestOrderType;
    CustAccount                custAccount;
    CurrencyCode               currencyCode;
    CustPurchaseOrder          custPurchaseOrder;
    CustRef                    custRef;
    ProdPoolId                 prodPoolId;
    ATXSeasonId                seasonId_AT;
    ATXDestinationPlaceId      destinationPlaceId_AT;
    ATXItemDivisionId          itemDivisionId_AT;
    ATXBranchId                branchId;
    ATXRequestOrderDate        requestOrderDate;
    ATXRequestOrderCancelDate  requestOrderCancelDate_AT;
    ItemId                     itemId;
    InventSiteId               inventSiteId;
    InventLocationId           inventLocationId;
    EcoResConfigurationName    configId;
    EcoResSizeName             inventSizeId;
    EcoResColorName            inventColorId;
    ATXSampleTypeId            sampleTypeId_AT;
    ATXQtyBase                 custQty;
    ATXRequestQty              reqQty;
    Price                      price;
    ATXCustPlanNumber          planNumber;
    ATXIssueDate               issueDate;
    InventTable                inventTable;


}FormRun&   " dialog Dialog�" dialogOption DialogField�" dialogFileOpen DialogField�" fieldApp DialogField�" availableTypes  	  �" okButtonName  	  �" fileUploadName  �" 	delimiter 	Delimiter�" textFile  �" text  �" 
lineNumber 
LineNumber�" captionGroup Caption�" recordInsertListErrors RecordInsertList�" requestOrderType ATXRequestOrderType�" custAccount CustAccount�" currencyCode CurrencyCode�" custPurchaseOrder CustPurchaseOrder�" custRef CustRef�" 
prodPoolId 
ProdPoolId�" seasonId_AT ATXSeasonId�" destinationPlaceId_AT ATXDestinationPlaceId�" itemDivisionId_AT ATXItemDivisionId�" branchId ATXBranchId�" requestOrderDate ATXRequestOrderDate�" requestOrderCancelDate_AT ATXRequestOrderCancelDate�" itemId ItemId�" inventSiteId InventSiteId�" inventLocationId InventLocationId�" configId EcoResConfigurationName�" inventSizeId EcoResSizeName�" inventColorId EcoResColorName�" sampleTypeId_AT ATXSampleTypeId�" custQty 
ATXQtyBase�" reqQty ATXRequestQty�" price Price�" 
planNumber ATXCustPlanNumber�" 	issueDate ATXIssueDate�" inventTable InventTable�   � 
initData   � _data  ��  � �� 	
main   � _args Args��  � �� 
updateQtyOV�  � �� 
validateData�  boolean� �� 
createRequest�  � �� 
insertErrorsInTable�  � �� 
initErrorList�  � �ATXRequestOrderUpload�� !     ExtensionOf        	BOMCreate� � � classStr���/// <summary>
/// Update BOM type on BOMCreate for Templates
/// </summary>
[ExtensionOf(classStr(BOMCreate))]
final class BOMCreate_Extension
{
    public container value;

}   " value  	 �   � 
createNewBom   � _bomId BOMId�� _itemGroupId ItemGroupId�� _dialogSiteId InventSiteId�� _dialogName Name�� _pmfIsFormula boolean��  BOMTable� �BOMCreate_Extension�� ! %class ATXRequestOrderNewVersion
{
}   � 	
main   � _args Args��  � �ATXRequestOrderNewVersion�� !     ExtensionOf        EcoResProductMasterDimension� � � formStr��n[ExtensionOf(formStr(EcoResProductMasterDimension))]
final class EcoResProductMasterDimension_Extension
{
}   �     FormControlEventHandler        EcoResProductMasterDimension� ATXButtonGridSize� � formControlStr�     Clicked�	 FormControlEventType��	
ATXButtonGridSize_OnClicked   � sender FormControl�� e FormControlEventArgs��  � ��     FormControlEventHandler        EcoResProductMasterDimension� ATXButtonGridColor� � formControlStr�     Clicked�	 FormControlEventType��	
ATXButtonGridColor_OnClicked   � sender FormControl�� e FormControlEventArgs��  � �&EcoResProductMasterDimension_Extension�� ! �/// <summary>
/// Authorize request order
/// Change status of RequestOrderHeader to Authorized
/// Create a new sales order
/// Group lines based on # dimensions
/// Create a new BOM for every group line
/// TODO Update header with style and qty?
/// TODO Sample WIP
/// </summary>
class ATXRequestOrderAuthorize extends ATXRequestOrder
{
    AxSalesTable    axSalesTable;
    SalesTable      salesTable;

}ATXRequestOrder   " axSalesTable AxSalesTable�" 
salesTable 
SalesTable�   � 	
main   � _args Args��  � �� 
run�  � �� 
validateAuthorize�  boolean� �� 
createWIPRecord�  � �� 
createSalesTable�  � �� 
createSalesLines�  ��� 	
validateRequestLines   � _requestOrderHeader ATXRequestOrderHeader��  boolean��ATXRequestOrderAuthorize�� ! �	class ATXProdRouteMultiRegisterProd
{
    ProdTable               prodTable;
    ProdRoute               prodRoute;
    ATXProdCutSection       prodCutSection_AT;
    ProdId                  prodId;
    BOMId                   bomId;
    ProdQtyCalc             qtyCalc;
    ATXRejectionCodeId      rejectionCode;
    ATXCutId                cutId;
    Noyes                   rejection;
    Noyes                   transferCheck;
    ATXTurnId               turnId;
    wrkCtrId                wrkCtrId;
    RouteOprId              oprId;
    ATXRouteOprTable        routeOprTable_AT;
    InventJournalTable      inventJournalTableTransfer;
    ItemId                  itemIdTransfer;
    ATXProdParameters       prodParameters;
    ATXProdRefComment       refComment;
    EcoResStyleName         inventStyleIdTransfer;
    EcoResConfigurationName configIdTransfer;
    EcoResColorName         inventColorIdTransfer;
    Hours                   shutDownIdHours, setupHours, execHours;
    Minutes                 shutDownIdMinutes, setupMinutes, execMinutes;
    Description             journalDescriptionStr = ATXProdParameters::find().JournalMovDescription;

    // Add empleyee number
    HcmPersonnelNumberId    hcmPersonnelNumberId;

}   " 	prodTable 	ProdTable�" 	prodRoute 	ProdRoute�" prodCutSection_AT ATXProdCutSection�" prodId ProdId�" bomId BOMId�" qtyCalc ProdQtyCalc�" rejectionCode ATXRejectionCodeId�" cutId ATXCutId�" 	rejection Noyes�" transferCheck Noyes�" turnId 	ATXTurnId�" wrkCtrId wrkCtrId�" oprId 
RouteOprId�" routeOprTable_AT ATXRouteOprTable�" inventJournalTableTransfer InventJournalTable�" itemIdTransfer ItemId�" prodParameters ATXProdParameters�" 
refComment ATXProdRefComment�" inventStyleIdTransfer EcoResStyleName�" configIdTransfer EcoResConfigurationName�" inventColorIdTransfer EcoResColorName�" shutDownIdHours Hours�" 
setupHours Hours�" 	execHours Hours�" shutDownIdMinutes Minutes�" setupMinutes Minutes�" execMinutes Minutes�" journalDescriptionStr Description�" hcmPersonnelNumberId HcmPersonnelNumberId�(   � 
parmHCMPersonnelNumberId   � hcmPersonnelNumberId_hcmPersonnelNumberId HCMPersonnelNumberId�� false_refresh boolean��  HCMPersonnelNumberId� �� 
resetScannedPersonnelNumberId�  � �� 
parmRejectionCode   � rejectionCode_rejectionCode ATXRejectionCodeId��  ATXRejectionCodeId� �� 
parmRejection   � 	rejection
_rejection Noyes��  Noyes� �� 

parmProdId   � prodId_prodId ProdId�� false_refresh boolean��  ProdId� �� 
resetScannedProdId�  � �� 
	parmOprId   � oprId_oprId 
RouteOprId�� false_refresh boolean��  
RouteOprId� �� 
getWrkCtrId�  ��� 
parmRouteOprTable_AT   � routeOprTable_AT_routeOprTable_AT ATXRouteOprTable��  ATXRouteOprTable� �� 
parmWrkCtrId   � wrkCtrId	_wrkCtrId WrkCtrId��  WrkCtrId� �� 
resetScannedOprId�  � �� 
	parmCutId   � cutId_cutId ATXCutId��  ATXCutId� �� 
parmProdCutSection_AT   � prodCutSection_AT_prodCutSection_AT ATXProdCutSection��  ATXProdCutSection� �� 
parmATXProdRefComment   � 
refComment_refComment ATXProdRefComment��  ATXProdRefComment� �� 
fillMultiRegister   � ""_wmsLocationId WMSLocationId��  ATXProductionFloorControl� �� 	
getSystemDate�   � �� 

parmTurnId   � turnId_turnId 	ATXTurnId��  	ATXTurnId� �� 
parmInventStyleIdTransfer   � inventStyleIdTransfer_inventStyleIdTransfer EcoResStyleName��  EcoResStyleName� �� 
parmProdRoute   � 	prodRoute
_prodRoute 	ProdRoute��  	ProdRoute� �� 
insertShutDownCode   � systemDateGet()
_transDate 	TransDate��  boolean� �� 
validateShutDownCode�  boolean��� 
validateFloorControlData   � null_fDS FormDataSource��  boolean� �� 
checkShutDownCodePosted�  boolean��� 
getShutDownCodeHours�  Hours��� 
parmShutDownIdHours   � shutDownIdHours_shutDownIdHours Hours��  Hours� �� 
parmShutDownIdMinutes   � shutDownIdMinutes_shutDownIdMinutes Minutes��  Minutes� �� 
&insertJournalRouteLineTimeWrkFromRoute   � 
_journalId 	JournalId�� _routeOprId 
RouteOprId�� _qty Qty�� RouteJobType::Process_routeJobType RouteJobType�� systemDateGet()
_transDate 	TransDate�� null_prodRouteConsumption ATXProdRouteMultiRegisterProd��  � �� 
canReportAsFinish   � _fds FormDataSource�� false_refresh boolean��  boolean� �� 
validatePostMulti   � _fDS FormDataSource��  boolean� �� 
postBackflush   � _fds FormDataSource��  ��� 
	postRoute   � _fds FormDataSource��  ��� 
parmTransferCheck   � transferCheck_transferCheck Noyes��  Noyes� �� 
postProd   � _fDS FormDataSource��  ��� 
parmConfigIdTransfer   � configIdTransfer_configIdTransfer EcoResConfigurationName��  EcoResConfigurationName� �� 
parmInventColorIdTransfer   � inventColorIdTransfer_inventColorIdTransfer EcoResColorName��  EcoResColorName� �� 
createInventJournalLines   � _prodJournalTable ProdJournalTable��  � �� 
parmItemIdTransfer   � itemIdTransfer_itemIdTransfer ItemId��  ItemId� �� 
createInventJournalTable�  inventJournalTable� �� 
updateStUpQty�  ��� 
postProdJournalProd   � _prodJournalTable ProdJournalTable�� false_validatePost boolean��  � �ATXProdRouteMultiRegisterProd�� ! [class ATXRequestOrderUpdateCustRef
{
    ATXRequestOrderHeader requestOrderHeaderParm;
}   " requestOrderHeaderParm ATXRequestOrderHeader�   � 	
main   � _args Args��  � �� 
run�  � �� 
parmRequestOrderHeader_AT   � requestOrderHeaderParm_requestOrderHeader_AT ATXRequestOrderHeader��  ATXRequestOrderHeader� �ATXRequestOrderUpdateCustRef�� ! �/// <summary>
/// Base class RequestOrder
/// </summary>
class ATXRequestOrder extends RunBase
{
    ATXRequestOrderHeader   requestOrderHeader;
    ATXRequestOrderUpdates  requestOrderUpdates;
    ATXRequestOrderUpdateId requestOrderUpdateId;
    Map                     recordMap;
    MapEnumerator           recordEnumerator;
    ATXRequestOrderId       requestOrderId;
    ATXRequestOrderType     requestOrderType;
    ATXRequestOrderStatus   requestOrderStatus;
    Dialog                  dialog;
    boolean                 infoMessages;
    FreeTxt                 messageTxt;

}RunBase   " requestOrderHeader ATXRequestOrderHeader�" requestOrderUpdates ATXRequestOrderUpdates�" requestOrderUpdateId ATXRequestOrderUpdateId�" 	recordMap Map�" recordEnumerator MapEnumerator�" requestOrderId ATXRequestOrderId�" requestOrderType ATXRequestOrderType�" requestOrderStatus ATXRequestOrderStatus�" dialog Dialog�" infoMessages boolean�" 
messageTxt FreeTxt�   � 
dialogPostRun   � 	tmpDialog DialogRunbase��  � �� 
initRecordsMap   � _args Args��  � �� 
parmInfoMessages   � infoMessages_infoMessages NoYesId��  NoYesId� �� 
parmMessageTxt   � 
messageTxt_messageTxt FreeText��  FreeText� �� 
parmRequestOrderHeader   � requestOrderHeader_requestOrderHeader ATXRequestOrderHeader��  ATXRequestOrderHeader� �� 
unpack   � packedClass  ��  boolean� �� 
parmRequestOrderType   � requestOrderType_requestOrderType ATXRequestOrderType��  ATXRequestOrderType� �� 
parmRequestOrderId   � requestOrderId_requestOrderId ATXRequestOrderId��  ATXRequestOrderId� �� 
parmRequestOrderStatus   � requestOrderStatus_requestOrderStatus ATXRequestOrderStatus��  ATXRequestOrderStatus� �� 
validateUpdate�  boolean� �� 
parmRequestOrderUpdateId   � requestOrderUpdateId_requestOrderUpdateId ATXRequestOrderUpdateId��  ATXRequestOrderUpdateId� �ATXRequestOrder�� ! &class ATXInventJournalMuilti
{
    }   � 
newInventJournalTable   � _journalType InventJournalType�� _description Description��  InventJournalTable� �� 
postInventJournal   � _inventJournalTable InventJournalTable�� false_validatePost boolean��  � �ATXInventJournalMuilti�� ! class ATXSalesBOMUpdate
{
}   � 
run   � 
_salesLine 	SalesLine��  ��� 	
main   � _args Args��  � �ATXSalesBOMUpdate�� ! �class ATXFormCanvasLog
{
    ATXTmpInfologError  tmpLog;
    FormDataSource      tmplogDS;
    str                 logMessage;
    int                 messageCounter;
    boolean             skipTmpInfologUpdate;

}   " tmpLog ATXTmpInfologError�" tmplogDS FormDataSource�" 
logMessage  �" messageCounter  �" skipTmpInfologUpdate boolean�   � 
clearInfologOrigin�  � �� 
dropTmpInfolog�  � �� 
parmTempLogDS   � tmpLogDS	_tmpLogDS FormDataSource��  FormDataSource� �� 
	playAlarm�  � �� 
updateInfologView   � false_forceNotAlarm boolean��  � �ATXFormCanvasLog�� ! dclass ATXTools
{
    #define.languageCodeEnUs('en-us')
    #define.languageCodeEsMx('es-mx')

}   � 	
fillWithChar   � _string  �� _length  �� ''
_character  ��   � �� 	
getSerialFromItem   � _itmeId ItemId��  inventSerialId� �� 	
createBatch   � _itemid ItemId�� _inventBatchId InventBatchId�� systemDateGet()	_prodDate 	TransDate��  � �� 	
reserveLine   � _common Common�� 
_inventdim 	Inventdim�� 
_qtyReserv Qty��  � �� 	
getLastProdOperation   � _prodId ProdId��  
RouteOprId� �� 	
fillWithCharLeft   � _string  �� _length  �� ''
_character  ��   � �� 	
fillWithCharRight   � _string  �� _length  �� ''
_character  ��   � �� 	
replaceChar   � _char  �� _fromStr  �� _toStr  ��   � �� 	
replaceControlChar   � _char  ��   � �� 	
replaceHTMLChar   � _char  ��   � �� 	
replaceEnterChar   � _char  ��   � �� 	
createProductMasterSize   � _inventTable InventTable�� _inventSizeId EcoResSizeName�� _description Description�� _retailDisplayOrder RetailDisplayOrder��  � �� 	
isBatchTrackingDimensionActive   � _itemId ItemId��  boolean� �� 	
isInventLocationIdActive   � _itemId ItemId��  boolean� �� 	
isInventSiteIdActive   � _itemId ItemId��  boolean� �� 	
isSerialTrackingDimensionActive   � _itemId ItemId��  boolean� �� 	
isWMSLocationIdActive   � _itemId ItemId��  boolean� �� 	
isWMSPalletIdActive   � _itemId ItemId��  boolean� �� 	
itemColorName   � _itemId ItemId�� _ecoResColorName EcoResColorName��  Description� �� 	
itemConfigurationName   � _itemId ItemId�� _ecoResConfigurationName EcoResConfigurationName��  Description� �� 	
itemSizeName   � _itemId ItemId�� _ecoResSizeName EcoResSizeName��  Description� �� 	
itemStyleName   � _itemId ItemId�� _ecoResStyleName EcoResStyleName��  Description� �� 	
oprNumFromRoute   � _itemId ItemId�� _oprId 
RouteOprId��  OprNum� �� 	
oprNumFromRouteNotActive   � _itemId ItemId�� _oprId 
RouteOprId��  OprNum� �� 	
updateStorageTrackingForced   � _itemId ItemId�� _storageGroup EcoResProductDimensionName�� _trackingGroup EcoResProductDimensionName��  � �� 	
existsConfiguration   � _inventTable InventTable�� 	_configId EcoResConfigurationName��  boolean� �� 	

existsSize   � _inventTable InventTable�� _inventSizeId EcoResSizeName��  boolean� �� 	
existsColor   � _inventTable InventTable�� _inventColorId EcoResColorName��  boolean� �� 	
existsStyle   � _inventTable InventTable�� _inventStyleId EcoResStyleName��  boolean� �� 	
copyGridToDim   � _inventTable InventTable�� _itemGridId ATXItemGridId�� _type ATXDimComboType��  � �� 	
createProductVariants   � _productMasterRecId EcoResProductMasterRecId�� _productDimensionAttribute RefRecId�� _productDimensionValue RefRecId��  � �ATXTools�� ! class ATXApproveTasks
{
}   � 	
main   � _args Args��  � �� 
run   � _productMasterSizeDS FormDataSource��  � �ATXApproveTasks�� ! {class ATXProdCutPatternQtyUpdate
{
    ATXProdCutPattern prodCutPattern_AT;
    ATXProdCutHeader  prodCutHeader_AT;

}   " prodCutPattern_AT ATXProdCutPattern�" prodCutHeader_AT ATXProdCutHeader�   � 	
main   � _args Args��  � �� 
runFromHeader�  � �� 
parmProdCutPattern_AT   � prodCutPattern_AT_prodCutPattern_AT ATXProdCutPattern��  ATXProdCutPattern� �� 
parmProdCutHeader_AT   � prodCutHeader_AT_prodCutHeader_AT ATXProdCutHeader��  ATXProdCutHeader� �ATXProdCutPatternQtyUpdate�� ! Sclass ATXRouteCardContract
{
    RefRecId recId;
    RouteOprId routeOprId;

}   " recId RefRecId�" 
routeOprId 
RouteOprId�   �     DataMemberAttribute    "RecId"�� &SysOperationControlVisibilityAttribute     False��
refRecId   � recId_recId RefRecId��  RefRecId� ��     DataMemberAttribute        
RouteOprId� � � extendedTypeStr��
parmRouteOprId   � 
routeOprId_routeOprId 
RouteOprId��  
RouteOprId� �ATXRouteCardContract�� ! �/// <summary>
/// Dialog class
/// Create a BOMVersion for every combination on InventDim of a product master
/// Type::Variant
/// </summary>
class ATXReleaseBOMVersionVariants extends RunBaseBatch
{
    BOMVersion BOMVersion;
    BOMId bomId;
    Dialog dialog;
    DialogField dflBOMId;

    #DEFINE.CurrentVersion(7)
    #LOCALMACRO.CurrentList
        bomId
    #endMacro

}RunBaseBatch   " 
BOMVersion 
BOMVersion�" bomId BOMId�" dialog Dialog�" dflBOMId DialogField�   � 
pack�   � �� 
unpack   � packedClass  ��  boolean� �� 
	parmBOMId   � bomId_bomId BOMId��  BOMId� �� 	
	construct�  ATXReleaseBOMVersionVariants� �� 
new�  � �� 
run�  � �� 	
main   � _args Args��  � �� 
dialog�  Object� �� 
getFromDialog�  boolean� �� 
parmBOMVersion   � 
bomVersion_bomVersion 
BOMVersion��  
BOMVersion� �� 
caption�  ClassDescription� �ATXReleaseBOMVersionVariants�� ! �/// <summary>
/// BOM Matrix funcions
/// </summary>
class ATXBOMMatrixEngine
{
    ATXBOMMatrixTemplate    bomMatrixTemplateOriginal;
    ATXBOMTemplateLine      bomTemplateLine;
    boolean                 configActive, sizeActive, colorActive, styleActive;
    ItemId                  productMasterItemId;

}   " bomMatrixTemplateOriginal ATXBOMMatrixTemplate�" bomTemplateLine ATXBOMTemplateLine�" configActive boolean�" 
sizeActive boolean�" colorActive boolean�" styleActive boolean�" productMasterItemId ItemId�   � 
createBOMLine   � _inventDimProductMaster 	InventDim��  ��� 
createBOMRecord   � _bomTemplateLine RefRecId�� _bomId BOMId�� _itemIdMatrix ItemId�� _bomConsumpType BOMConsumpType�� _bomQty BOMQty�� _bomQtySerie BOMQtySerie�� 
_bomUnitId 	BOMUnitId�� _routeOprId 
RouteOprId�� _inventDimId InventDimId�� _scrapConst 
ScrapConst�� 	_scrapVar ScrapVar�� _configIdStyle EcoResConfigurationName�� _inventSizeIdStyle EcoResSizeName�� _inventColorIdStyle EcoResColorName�� _inventStyleIdStyle EcoResStyleName�� _bomType BOMType�� _vendAccount VendAccount�� 	_seasonId ATXSeasonId�� _destinationPlaceId ATXDestinationPlaceId��  ��� 
createBOMLineBySize   � _inventDimProductMaster 	InventDim�� _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
createBOMLineByStyleColor   � _inventDimProductMaster 	InventDim�� _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
createBOMLineByStyleColorSize   � _inventDimProductMaster 	InventDim�� _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
createBOMLineNoDimByStyleDim   � _inventDimProductMaster 	InventDim�� _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
createBOMLineSameColorSize   � _inventDimProductMaster 	InventDim�� _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
 generateCombinationSameSizeColor   � _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
generateStyleCombinations�  ��� 
generateStyleLinesBySize   � _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
generateStyleLinesBySizeMatrix   � _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
initDimActive   � _inventDimProductMaster 	InventDim��  ��� 
parmBomMatrixTemplateOriginal   � bomMatrixTemplateOriginal_bomMatrixTemplateOriginal ATXBOMMatrixTemplate��  ATXBOMMatrixTemplate� �� 
parmBOMTemplateLine   � bomTemplateLine_bomTemplateLine ATXBOMTemplateLine��  ATXBOMTemplateLine� �� 
parmProductMasterItemId   � productMasterItemId_itemId ItemId��  ItemId� �� 
run�  ��� 
updateBOMLineBySize   � _bomMatrixTemplate ATXBOMMatrixTemplate��  ��� 
validateData�  ��� 	
main   � _args Args��  � �ATXBOMMatrixEngine�� ! Cclass ATXRouteCardController extends SrsReportRunController
{

}SrsReportRunController   � 	
main   � _args Args��  � �� 
prePromptModifyContract�  � �ATXRouteCardController�� ! �/// <summary>
/// Contains all functions to create BOMVersions
/// TODO Falta funcionalidad para actualizar listas de materiales de OV y OP
/// </summary>
class ATXBOMVersionEngine
{
    BOMId                   templateBOMId;
    ItemId                  templateItemId;
    BOMVersion              templateBOMVersion;
    NumberOfRecords         numberOfRecords;
    SysOperationProgress    sysProgress;
    ItemId                  itemId;
    BOMConsumpType          bomConsumpType;
    EcoResColorName         inventColorId;
    #AviFiles
    #ATXBOMMacro

    

}   " templateBOMId BOMId�" templateItemId ItemId�" templateBOMVersion 
BOMVersion�" numberOfRecords NumberOfRecords�" sysProgress SysOperationProgress�" itemId ItemId�" bomConsumpType BOMConsumpType�" inventColorId EcoResColorName�   � 
new   � _bomId BomId�� _itemId ItemId��  � �� 	
generateVariantBOMVersions   � _bomId BOMId�� _itemId ItemId��  � �� 
run�  � �� 
generateVersionsHeaders�  ��� 	

getBOMName   � _itemId ItemId�� 
_inventDim 	InventDim��  Name� �� 	
createBOMTable   � _itemId ItemId�� _name Name�� ATXBOMType::None_bomType 
ATXBOMType�� ""_bomId BOMId�� ""_inventSiteId InventSiteId��  BOMId� �� 	
findVariantVersion   � _itemId ItemId�� 	_configId EcoResItemConfigurationName�� _inventColorId EcoResItemColorName�� _InventSizeId EcoResItemSizeName�� _inventStyleId EcoResItemStyleName�� false
_forUpdate boolean��  
BOMVersion� �� 	
findEcoResProductMasterColor   � _productMaster RefRecId�� _colorRecId EcoResColorRecId�� "fieldnum(InventDim, InventcolorId)_inventDimFieldId fieldId�� false
_forupdate boolean��  EcoResProductMasterColor� �� 	
findEcoResProductMasterSize   � _productMaster RefRecId�� 
_sizeRecId EcoResSizeRecId�� !fieldnum(InventDim, InventSizeId)_inventDimFieldId fieldId�� false
_forupdate boolean��  EcoResProductMasterSize� �� 	
findEcoResProductMasterStyle   � _productMaster RefRecId�� _styleRecId EcoResSizeRecId�� "fieldnum(InventDim, InventStyleId)_inventDimFieldId fieldId�� false
_forupdate boolean��  EcoResProductMasterStyle� �� 	
findByItemBOMId   � _itemId ItemId�� _BOMId BOMId�� false
_forupdate boolean��  
BOMVersion� �ATXBOMVersionEngine�� ! �class ATXBOMTemplateEngine
{
    ATXBOMTemplateLine  bomTemplateLine;
    BOMId               bomId;
    ItemId              itemIdBOMVersion;
    NoYesId             singleLine;
    boolean             matrixConfig;

    NoYesId             configActive, sizeActive, colorActive, styleActive;
    AxdRecordAction     recordAction;

}
   " bomTemplateLine ATXBOMTemplateLine�" bomId BOMId�" itemIdBOMVersion ItemId�" 
singleLine NoYesId�" matrixConfig boolean�" configActive NoYesId�" 
sizeActive NoYesId�" colorActive NoYesId�" styleActive NoYesId�" recordAction AxdRecordAction�   � 
new   � _bomTemplateLine ATXBOMTemplateLine�� false_matrixConfig boolean��  � �� 
parmBOMTemplateLine   � bomTemplateLine_bomTemplateLine ATXBOMTemplateLine��  ATXBOMTemplateLine� �� 
	parmBOMId   � bomId_bomId BOMId��  BOMId� �� 
updateFromDoApply�  � �� 
initParmsFromBOMTemplateLine   � _bomTemplateLine ATXBOMTemplateLine��  ��� 
parmColorActive   � colorActive_colorActive NoYesId��  NoYesId� �� 
parmConfigActive   � configActive_configActive NoYesId��  NoYesId� �� 
parmSizeActive   � 
sizeActive_sizeActive NoYesId��  NoYesId� �� 
parmStyleActive   � styleActive_styleActive NoYesId��  NoYesId� �� 
insertOrUpdateBOMLine�  ��� 
checkRecordAction�  ��� 
parmAxdRecordAction   � recordAction_recordAction AxdRecordAction��  AxdRecordAction� �� 
createBOMLine�  ��� 
!insertBOMLineFromProductMasterDim   � 
_inventDim 	InventDim��  ��ATXBOMTemplateEngine�� ! mclass ATXAXRequestOrderHeader extends AxInternalBase
{
    ATXRequestOrderHeader   requestOrderHeader;

}AxInternalBase   " requestOrderHeader ATXRequestOrderHeader�   � 
currentRecord   � requestOrderHeader_requestOrderHeader Common��  Common� �� 
parmProdPoolId   � ''_prodPoolId 
ProdPoolId��  
ProdPoolId� �� 
parmRequestOrderCancelDate_AT   � EDateTimeUtil::getSystemDate(DateTimeUtil::getUserPreferredTimeZone())_requestOrderCancelDate ATXRequestOrderCancelDate��  ATXRequestOrderCancelDate� �� 
emptyRecord�  Common� �� 
new�  � �� 
parmCurrencyCode   � ''_currencyCode CurrencyCode��  CurrencyCode� �� 
parmCustAccount   � ''_custAccount CustAccount��  CustAccount� �� 
parmCustPurchaseOrder   � ''_custPurchaseOrder CustPurchaseOrder��  CustPurchaseOrder� �� 
parmCustRef   � ''_custRef CustRef��  CustRef� �� 
parmInventLocationId   � ''_inventLocationId InventLocationId��  InventLocationId� �� 
parmInventSiteId   � ''_inventSiteId InventSiteId��  InventSiteId� �� 
parmInventTransType   � InventTransType::Production_inventTransType InventTransType��  InventTransType� �� 	
	construct�  ATXAXRequestOrderHeader� �� 
parmRequestOrderId_AT   � ''_requestOrderId ATXRequestOrderId��  ATXRequestOrderId� �� 
parmRequestOrderStatus_AT   � ATXRequestOrderStatus::Loaded_requestOrderStatus ATXRequestOrderStatus��  ATXRequestOrderStatus� �� 
parmRequestOrderGroupId_AT   � ''_RequestOrderGroupId_AT ATXRequestOrderGroupId��  ATXRequestOrderGroupId� �� 
parmRequestOrderCreated_AT   � 
dateNull()_requestOrderCreated ATXRequestOrderCreated��  ATXRequestOrderCreated� �� 
parmRequestOrderDate   � EDateTimeUtil::getSystemDate(DateTimeUtil::getUserPreferredTimeZone())_requestOrderDate ATXRequestOrderDate��  ATXRequestOrderDate� �� 
parmRequestOrderType_AT   � ATXRequestOrderType::Sales_requestOrderType ATXRequestOrderType��  ATXRequestOrderType� �� 
requestOrderHeader   � requestOrderHeader_requestOrderHeader ATXRequestOrderHeader��  ATXRequestOrderHeader� �ATXAXRequestOrderHeader�� ! �class ATXRequestOrderCreate extends ATXRequestOrder
{
    DialogField                 dialogRequestOrderId,
                                dialogRequestOrderType,
                                dialogCustAccount,
                                dialogCurrencyCode,
                                dialogCustPurchaseOrder,
                                dialogCustRef,
                                dialogProdPoolId,
                                dialogRequestOrderGroupId_AT,
                                dialogInventTransType,
                                dialogRequestOrderCreated,
                                dialogInventSiteId,
                                dialogInventLocationId,
                                dialogRequestOrderDate,
                                dialogRequestOrderCancelDate,
                                dialogSampleTypeId;

    CustAccount                 custAccount;
    CurrencyCode                currencyCode;
    CustPurchaseOrder           custPurchaseOrder;
    CustRef                     custRef;
    ProdPoolId                  prodPoolId;
    InventTransType             inventTransType;
    ATXRequestOrderCreated      requestOrderCreated;
    ATXRequestOrderDate         requestOrderDate;
    ATXRequestOrderCancelDate   requestOrderCancelDate;
    ATXRequestOrderGroupId      requestOrderGroupId_AT;
    InventSiteId                inventSiteId;
    InventLocationId            inventLocationId;
    ATXSampleTypeId             sampleTypeId_AT;

    #define.RequestOrderNumberDefault(1)

}ATXRequestOrder   " dialogRequestOrderId DialogField�" dialogRequestOrderType DialogField�" dialogCustAccount DialogField�" dialogCurrencyCode DialogField�" dialogCustPurchaseOrder DialogField�" dialogCustRef DialogField�" dialogProdPoolId DialogField�" dialogRequestOrderGroupId_AT DialogField�" dialogInventTransType DialogField�" dialogRequestOrderCreated DialogField�" dialogInventSiteId DialogField�" dialogInventLocationId DialogField�" dialogRequestOrderDate DialogField�" dialogRequestOrderCancelDate DialogField�" dialogSampleTypeId DialogField�" custAccount CustAccount�" currencyCode CurrencyCode�" custPurchaseOrder CustPurchaseOrder�" custRef CustRef�" 
prodPoolId 
ProdPoolId�" inventTransType InventTransType�" requestOrderCreated ATXRequestOrderCreated�" requestOrderDate ATXRequestOrderDate�" requestOrderCancelDate ATXRequestOrderCancelDate�" requestOrderGroupId_AT ATXRequestOrderGroupId�" inventSiteId InventSiteId�" inventLocationId InventLocationId�" sampleTypeId_AT ATXSampleTypeId�	   � 
createRequestOrder�  ��� 
validate   � null
calledFrom Object��  boolean� �� 
dialog�  Object� �� 
Fld2_1_modified�  boolean� �� 
Fld3_1_modified�  boolean� �� 
Fld12_1_modified�  boolean� �� 
getFromDialog�  boolean� �� 
run�  � �� 	
main   � _args Args��  � �ATXRequestOrderCreate�� ! yclass ATXPmfFormCtrl_BOMTemplateEdit extends PmfFormCtrl
{
    InventDim   inventDim;
    BOMVersion  bomVersion;

}PmfFormCtrl   " 	inventDim 	InventDim�" 
bomVersion 
BOMVersion�   � 
bomLine�  ATXBOMTemplateLine��� 
canModifyBOM�  boolean��� 
dataSourceInitValuePost   � _buffer Common��  � �� 
dataSourceValidateWrite�  boolean� �� 
fieldLookup   � _fieldId fieldId�� _formControl FormControl�� 
_filterStr  ��  � �� 
initPost�  � �� 
isFormulaEnabled�  boolean� �� 
parmBOMVersion   � 
bomVersion_bomVersion 
BOMVersion��  
BOMVersion� �� 
parmInventDim   � 	inventDim
_inventDim 	InventDim��  	InventDim� �� 
setDatasources   � buffer_datasources1 Common�� null_datasources2 Common�� null_datasources3 Common�� null_datasources4 Common�� null_datasources5 Common��  � �� 	
	construct�  ATXPmfFormCtrl_BOMTemplateEdit� �� 	
newFromForm   � _fr FormRun��  ATXPmfFormCtrl_BOMTemplateEdit� �ATXPmfFormCtrl_BOMTemplateEdit�� ! �class ATXRequestOrderCopy extends RunBase
{
    DialogField             dlgFromCustPurchaseOrder,
                            dlgFromCustRef,
                            dlgToCustPurchaseOrder,
                            dlgToCustRef;

    ATXRequestOrderHeader   requestOrderHeader;

    CustPurchaseOrder       custPurchaseOrder;
    CustRef                 custRef;


}RunBase   " dlgFromCustPurchaseOrder DialogField�" dlgFromCustRef DialogField�" dlgToCustPurchaseOrder DialogField�" dlgToCustRef DialogField�" requestOrderHeader ATXRequestOrderHeader�" custPurchaseOrder CustPurchaseOrder�" custRef CustRef�   � 	
main   � _args Args��  � �� 
run�  � �� 
parmRequestOrderHeader   � requestOrderHeader_requestOrderHeader ATXRequestOrderHeader��  ATXRequestOrderHeader� �� 
parmCustRef   � custRef_custRef CustRef��  CustRef� �� 
unpack   � packedClass  ��  boolean� �� 
parmCustPurchaseOrder   � custPurchaseOrder_custPurchaseOrder CustPurchaseOrder��  CustPurchaseOrder� �� 
getFromDialog�  boolean� �� 
dialog�  Object� �ATXRequestOrderCopy�� ! ?class ATXBreakdownOrderEngine
{
    SalesLine salesLine;

}   " 	salesLine 	SalesLine�
   � 	
getDummyInventDim   � _itemId ItemId�� _prodPoolSetup_AT ATXProdPoolSetup�� 	_configId EcoresConfigurationName�� _inventSizeId EcoresSizeName�� _inventColorId EcoresColorName�� _inventStyleId EcoResStyleName�� _inventSiteId InventSiteId�� _inventLocationId InventLocationId��  	InventDim� �� 
createBreakdownForSalesLineItem   � _requestOrderId ATXRequestOrderId�� _requestOrderUpdateId ATXRequestOrderUpdateId�� _itemId ItemId�� 
_inventDim 	InventDim��  � �� 
getInventDimFromVersion�  	InventDim��� 

insertLine   � _bom BOM��  boolean��� 
new   � _common Common��  � �� 
validateBuildBOM�  boolean��� 	
getDummiInventdim   � _itemId ItemId�� 	_configId EcoresConfigurationName�� _inventSizeId EcoresSizeName�� _inventColorId EcoresColorName�� _inventStyleId EcoResStyleName�� _inventSiteId InventSiteId�� _inventLocationId InventLocationId��  	InventDim� �� 
buildProdBOMFromTemplate�  BOMId� �� 
insertLineFromTemplate   � _breakOrderLine ATXBreakdownOrderLine�� _templateBOM BOM�� 
_salesLine 	SalesLine��  boolean� �� 	
findBOMLineVariant   � _bomId BOMId�� _itemId ItemId�� _inventDimId InventDimId�� _oprNum OprNum�� _oprId 
RouteOprId�� false
_forupdate boolean��  BOM� �ATXBreakdownOrderEngine�� !     ExtensionOf        	SalesLine� � � tableStr��L[ExtensionOf(tableStr(SalesLine))]
final class ATXSalesLine_Extension
{
}   � 	
atxFindItemDim   � _salesId SalesId�� _itemId ItemId�� 
_inventDim 	InventDim�� _origInventTransId InventTransId�� false
_forupdate boolean��  	salesline� �ATXSalesLine_Extension�� !     ExtensionOf        
SalesTable� � � tableStr��R[ExtensionOf(tableStr(SalesTable))]
final public class SalesTable_Extension
{
}   � 
delete�  � �� 
deleteRequestOrderReference�  � ��     DataEventHandler        
SalesTable� � � tableStr�     ValidatedDelete�	 DataEventType��	
SalesTable_onValidatedDelete   � sender Common�� e DataEventArgs��  � �SalesTable_Extension�� !     ExtensionOf        BOMCreateDialog� � � classStr���/// <summary>
/// Add a new field to enable Template type
/// </summary>
[ExtensionOf(classStr(BOMCreateDialog))]
final class BOMCreateDialog_Extension
{
    public NoYes        atxTemplateActive;
    public DialogField  atxFieldTemplateActive;

}   " atxTemplateActive NoYes	 �" atxFieldTemplateActive DialogField	 �   � 
promptCreateBOMDialog   � _manual boolean�� _pmfIsFormula boolean��   � �BOMCreateDialog_Extension�� ! Eclass ATXInventDimCtrl_Frm_ProductDim extends InventDimCtrl_Frm
{
}InventDimCtrl_Frm   � 	
newFromForm   � _formRun FormRun��  ATXInventDimCtrl_Frm_ProductDim� �� 
mustEnableField   � _dimFieldId FieldId��  NoYes� �� 
mustShowGridField   � _dimFieldId FieldId��  NoYes� �� 
new�  � �� 
setupShowAllProductDimensions�  boolean� �� 	
	construct�  ATXInventDimCtrl_Frm_ProductDim� �ATXInventDimCtrl_Frm_ProductDim�� ! �class ATXRequestOrderCancel extends RunBase
{
    Args args;

    DialogField dfRequestOrderId, dialogCustPurchaseOrder;
    ATXRequestOrderId requestOrderId;
    CustPurchaseOrder custPurchaseOrder;

}RunBase   " args Args�" dfRequestOrderId DialogField�" dialogCustPurchaseOrder DialogField�" requestOrderId ATXRequestOrderId�" custPurchaseOrder CustPurchaseOrder�   � 
run�  � �� 
parmArgs   � args_args Args��  Args� �� 	
main   � _args Args��  � �� 
unpack   � packedClass  ��  boolean� �� 
getFromDialog�  boolean� �� 
dialog�  Object� �ATXRequestOrderCancel�� !  class ATXLookupTableEngine
{
}   � 	
lookupProdRoute   � _formControl FormControl�� _prodId ProdId��  � �� 	
lookupProdRouteName   � _formControl FormControl�� _prodId ProdId��  � �� 	
lookUpByParameters   � _formControl FormControl�� 
_tablename  �� _resultField  �� _fields4Range  �� _fieldsValue  �� 	connull()_fieldsToShow  ��  � �� 	
lookUpByParametersNum   � _formControl FormControl�� 
_tablename  �� _resultField  �� _fields4Range  �� _fieldsValue  �� 	connull()_fieldsToShow  ��  � �ATXLookupTableEngine�� !     ExtensionOf        ProdJournalCheckPostProd� � � classStr��j[ExtensionOf(classStr(ProdJournalCheckPostProd))]
final class ATXProdJournalCheckPostProd_Extension
{
}   �     PostHandlerFor        ProdJournalCheckPostProd� � � classStr�     ProdJournalCheckPostProd� run� � 	methodStr��	
!ProdJournalCheckPostProd_Post_run   � args XppPrePostArgs��  � �%ATXProdJournalCheckPostProd_Extension�� ! �class ATXRequestBOMGenerateBatch extends RunBaseBatch
{
    ATXRequestOrderHeader requestOrderHeader_AT;
    SalesId salesId;
    Dialog dialog;
    DialogField dflSalesId;

    #DEFINE.CurrentVersion(7)

    #LOCALMACRO.CurrentList
        salesId
    #endMacro

}RunBaseBatch   " requestOrderHeader_AT ATXRequestOrderHeader�" salesId SalesId�" dialog Dialog�" 
dflSalesId DialogField�   � 
pack�   � �� 
unpack   � packedClass  ��  boolean� �� 
parmSalesId   � salesId_salesId SalesId��  SalesId� �� 	
	construct�  ATXRequestBOMGenerateBatch� �� 
new�  � �� 
run�  � �� 	
main   � _args Args��  � �� 
dialog�  Object� �� 
getFromDialog�  boolean� �� 
parmRequestOrderHeader_AT   � requestOrderHeader_AT_requestOrderHeader_AT ATXRequestOrderHeader��  ATXRequestOrderHeader� �� 
caption�  ClassDescription� �ATXRequestBOMGenerateBatch�� ! class ATXUnApproveTasks
{
}   � 	
main   � _args Args��  � �� 
run   � _productMasterSizeDS FormDataSource��  � �ATXUnApproveTasks�� ! class ATXProductTools
{
}   � 	
existsConfiguration   � _inventTable InventTable�� 	_configId EcoResConfigurationName��  boolean� �� 	
isBatchTrackingDimensionActive   � _itemId ItemId��  boolean� �� 	
isSerialTrackingDimensionActive   � _itemId ItemId��  boolean� �� 	

existsSize   � _inventTable InventTable�� _inventSizeId EcoResSizeName��  boolean� �� 	
existsColor   � _inventTable InventTable�� _inventColorId EcoResColorName��  boolean� �ATXProductTools�� !     ExtensionOf        ReqTransPoMarkFirm� � � classStr���/// <summary>
/// 
/// </summary>
[ExtensionOf(classStr(ReqTransPoMarkFirm))]
final class ATXReqTransPOMarkFirm_Extension
{
}   � 
createProdTable   � 	_reqTrans ReqTrans�� _reqPO ReqPO�� _prodBOMParent ProdBOM��  	ProdTable� �ATXReqTransPOMarkFirm_Extension�� !     ExtensionOf        WrkCtrResourceGroupCalendar� � � tableStr��p[ExtensionOf(tableStr(WrkCtrResourceGroupCalendar))]
final class ATXWrkCtrResourceGroupCalendar_Extension
{
}   � 	
findActiveForResourceGroup   � _resourceGroup RefRecId�� _date  �� false
_forUpdate boolean��  WrkCtrResourceGroupCalendar� �(ATXWrkCtrResourceGroupCalendar_Extension�� ! �class ATXProdJournalMulti
{
    ProdJournalTable    prodJournalTable;
    ProdId              prodId;
    ProdJournalType     prodJournalType;

    

}   " prodJournalTable ProdJournalTable�" prodId ProdId�" prodJournalType ProdJournalType�   � 
newProdJournalTable   � _prodId ProdId�� _prodJournalType ProdJournalType�� _description Description��  ProdJournalTable� �� 
#insertJournalRouteLineFromProdRoute   � 
_journalId 	JournalId�� _routeOprId 
RouteOprId�� _qty Qty�� _bomId BOMId�� 	_wkrCtrId WrkCtrId�� RouteJobType::Process_routeJobType RouteJobType�� systemDateGet()
_transDate 	TransDate�� 0_hours ProdReportedHours�� ""
_turnId_AT 	ATXTurnId�� false
_rejection boolean�� ""_rejectionCodeId ATXRejectionCodeId�� false_isQualityLinetmp boolean�� ""_hcmPersonnelNumberId HcmPersonnelNumberId�� ""_cutId ATXCutId�� ""_comment ATXProdRefComment��  � �� 
postProdJournalRoute   � _prodJournalTable ProdJournalTable�� false_validatePost boolean��  � �� 
#inserProdJournalProdLineFromControl   � 
_journalId 	JournalId�� _qty ProdReportedGood�� _bomId BomId�� _quality ATXProdQualityId�� systemDateGet()
_transDate 	TransDate�� false
_rejection boolean�� null_productionFloorControl ATXProductionFloorControl�� null_prodRouteMultiRegistreProd ATXProdRouteMultiRegisterProd��  boolean� �� 
postProdJournalProd   � _prodJournalTable ProdJournalTable�� false_validatePost boolean��  � �ATXProdJournalMulti�� ! �// TODO Eliminar clase
class ATXBOMVersionVariants
{
    BOMVersion              templateBOMVersion;
    ItemId                  templateItemId;
    EcoResColorName         inventColorId;
    #AviFiles
    #ATXBOM

}   " templateBOMVersion 
BOMVersion�" templateItemId ItemId�" inventColorId EcoResColorName�   � 	
getBOMId�  BOMId� �� 	
getBOMNameFromSalesLine   � 
_salesLine 	SalesLine��  BOMId� �� 
approveBOMVersions�  ��� 	
approveBOMVersion   � _bomVersion 
BOMVersion��  � �ATXBOMVersionVariants�� !     ExtensionOf        
BOMVersion� � � tableStr��N[ExtensionOf(tableStr(BOMVersion))]
final class ATXBOMVersion_Extension
{
}   � 	
ATXfindByItemBOMId   � _itemId ItemId�� _bomId BOMId�� false
_forupdate boolean��  
BOMVersion� �ATXBOMVersion_Extension�� !     SRSReportParameterAttribute        ATXRouteCardContract� � � classStr���[SRSReportParameterAttribute(classStr(ATXRouteCardContract))]
class ATXRouteCardDP extends SRSReportDataProviderBase
{
    ATXRouteCardHeaderTmp      routeCardHeader;
    ATXRouteCardBreakdownTmp   routeCardBreakdown;
    ATXRouteCardRouteTmp       routeCardRoute;
    ProdTable                  prodTable;
    RouteOprId                 routeOprId;

}SRSReportDataProviderBase   " routeCardHeader ATXRouteCardHeaderTmp�" routeCardBreakdown ATXRouteCardBreakdownTmp�" routeCardRoute ATXRouteCardRouteTmp�" 	prodTable 	ProdTable�" 
routeOprId 
RouteOprId�   � 
processReport�  � �� 
insertHeader   � 
_prodTable 	ProdTable��  ��� 
insertBreackOrderLines   � 
_prodTable 	ProdTable��  ��� 
insertRoute   � 
_prodTable 	ProdTable��  ���     SrsReportDataSetAttribute        ATXRouteCardHeaderTmp� � � tableStr��
getRouteCardHeaderTmp�  ATXRouteCardHeaderTmp� ��     SrsReportDataSetAttribute        ATXRouteCardBreakdownTmp� � � tableStr��
getRouteCardBreakdownTmp�  ATXRouteCardBreakdownTmp� ��     SrsReportDataSetAttribute        ATXRouteCardRouteTmp� � � tableStr��
getRouteCardRouteTmp�  ATXRouteCardRouteTmp� �ATXRouteCardDP�� !     ExtensionOf        InventDimParm� � � tableStr��Q[ExtensionOf(tableStr(InventDimParm))]
final class InventDimParm_Extension
{
}   � 
atxInitDimBOMTemplateLineEnable   � _inventDimGroupSetup InventDimGroupSetup�� _bomLine ATXBOMTemplateLine��  � �InventDimParm_Extension�� ! �/// <summary>
/// Grid functionality
/// </summary>
class ATXItemGridEngine
{
    EcoResProductMaster ecoResProductMaster;

}   " ecoResProductMaster EcoResProductMaster�   � 
new   � _ecoResProductMasterParm EcoResProductMaster��  � �� 
copyDimensions   � _fDS FormDataSource�� _dimComboType ATXDimComboType��  � �� 
insertFromConfiguration   � _fDS FormDataSource��  � �� 
insertFromSize   � _fDS FormDataSource��  � �� 
insertFromColor   � _fDS FormDataSource��  � �� 
insertFromStyle   � _fDS FormDataSource��  � �ATXItemGridEngine�� ! �class ATXInventMovement
{
    ProdTable               prodTable;
    ProdJournalTable        prodJournalTable;
    boolean                 reverseMovement;
    Map                     salesLineMap;

}   " 	prodTable 	ProdTable�" prodJournalTable ProdJournalTable�" reverseMovement boolean�" salesLineMap Map�   � 
new   � _prodJournalTable ProdJournalTable�� false_reverse boolean��  � �� 
run�  � �� 
updateSalesLine�  � �� 
createSalesLine   � _prodJournalProd ProdJournalProd��  ��� 
updateBreakownFinished   � 
_salesLine 	SalesLine�� _prodJournalProd ProdJournalProd��  ��� 
removeSalesLine   � _prodJournalProd ProdJournalProd��  ��� 
transferJournal�  ��� 	
transferJournalReversal   � _prodJournalTable ProdJournalTable��  � �ATXInventMovement�