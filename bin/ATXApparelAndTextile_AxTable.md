I   ATXSampleWIP�tg5    �  ATXProductionFloorControl�tg5�  c  ATXBranchTable�tg51  �  ATXRequestOrderUpdates�tg5  �  ATXItemGridTable�tg5�  !  ATXProdCutPatternBreakdown�tg5  �  ATXProductPreProdTask�tg5�*  A  ATXBOMBlockingLogTable�tg5�/  �  ATXRequestOrderRelease�tg5~3  (  ATXRouteCardBreakdownTmp�tg5�5  �   ATXCutTechnicalSheet�tg5�6  A  ATXRejectionCodeTable�tg5�9  |  ATXSalesParameters�tg5Y<  C  ATXEventWarningParameters�tg5�@  K  ATXSubOperation�tg5�G    ATXProdQualityDimFieldSetUp�tg5�I  `  ATXPreProdTaskTemplate�tg5VM  �  ATXItemCategoryTable�tg5P  3  ATXDestinationPlace�tg5FS  �  ATXRouteOprTable�tg5)V  �  ATXCutTechnicalSheetWash�tg5�Y  �  ATXSalesParametersStaging�tg5�_  X  ATXProdCutPattern�tg5�c  ^  ATXProductParameters�tg5Jh  �  ATXApparelAndTextileParameters�tg5�j  �  ATXRouteCardHeaderTmp�tg5�l  �  ATXLineOfBusinessBOMBatch�tg5�n  �  ATXPlacementTable�tg5�p  �  ATXSampleBookTable�tg58s  �  ATXCutTechnicalSheetApp�tg5w  �  ATXProdCutSection�tg5{  �  ATXProdParameters�tg5��  �  ATXBrandTable�tg59�  �  ATXItemGridLines�tg5$�  �  ATXProdPoolSetup�tg5�    ATXRequestOrderHeader�tg5�  �  ATXProductParametersStaging�tg5	�  �  ATXBOMTemplateLine�tg5�  r  ATXInventItemPattern�tg5\�  �  ATXBOMMatrixTemplate�tg5��  N   ATXRequestOrderHeaderDataStaging�tg5M�  �
  ATXCutTechnicalSheetInterlining�tg5��  �  ATXRequestOrderUsers�tg5��  R  ATXProdCutHeader�tg5�  k  ATXEmailWarnings�tg5��  �  ATXRequestOrderGroupTable�tg5�  �  ATXSamplingPhase�tg5��  �  ATXBOMTypeTable�tg5��  "  ATXProdCutPackagesPost�tg5��  g  ATXSpreadingTable�tg5�  �  ATXSeasonTable�tg5��  �  ATXWorkCalendarDataStaging�tg5��  �  ATXSewStitchesPerInch�tg5\�  �  ATXSampleTypeTable�tg5��  �  ATXRouteSubOperationsAttributes�tg5��  Z  ATXEventWarningsGroup�tg5 {  ATXBreakdownOrderLine�tg5�   ATXProdCutPackages�tg5� 	  ATXPreProdTask�tg5� �  ATXTmpInfoLogError�tg5  9  ATXCutTechnicalSheetEmbroidery�tg5Y �  ATXBOMBlockingTable�tg5�   ATXItemDivisionTable�tg5� �  ATXTurnTable�tg5� �  ATXRequestOrderLine�tg5Z  �  ATXProductOvercutSetup�tg5'-   ATXEventWarningMailList�tg5<1 �  ATXProductOvercut�tg573 �  ATXProdQualityTable�tg5 6 �  ATXSewOperationMeasurements�tg5�8 �  ATXCustClassTable�tg5B> �  ATXRouteSubOperations�tg5�@ u  ATXRouteCardRouteTmp�tg5ZD   � �ATXPLM.public class ATXSampleWIP extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �RequestOrderId��SampleTypeId��CustAccount��CustPurchaseOrder��ItemId�	@SYS35893General�   �  	ATXRequestOrderId RequestOrderId��  	CustPurchaseOrderCustPurchaseOrder��	ItemIdItemId��	CustAccountCustAccount��	ATXSampleTypeIdSampleTypeId�!ATXSampleWIP9  ��� �;public class ATXProductionFloorControl extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �InventSizeId��QtySetUp��QtyPreviousOpr��	QtyPosted��Qty��
difference��Percent�
InventSize��   �InventSizeId��QtySetUp��Qty�InventStyle��   �ConfigId��InventColorId��InventSizeId��ProdQualityId��InventLocationId��WMSLocationId��QtyOrig��QtySetUp��QtyPreviousOpr��QtyPreviousOprError��	QtyPosted��ProdReportedError��Qty��
difference��Percent��	TransDate�ReportAsFinish�   �	BOMIdBOMId��	EcoResConfigurationNameConfigId��	EcoResColorNameInventColorId��	InventLocationIdInventLocationId��	EcoResSizeNameInventSizeId��	EcoResSizeNameInventSizeIdTransfer��	EcoResStyleNameInventStyleId��	ItemIdItemId��	
RouteOprIdOprId��OprNumOprNum��	ProdIdProdId��	ATXProdQualityIdProdQualityId��ProdReportedErrorProdReportedError��NumberOf@ATXAT:NewLabel145ProdStandarPack��QtyQty��    
ATXQtyOrigQtyOrig��ATXQtyPosted	QtyPosted��
ATXQtyBase@ATXAT:NewLabel148QtyPreviousOpr��	ATXCutQtyQtySetUp��	WMSLocationIdWMSLocationId��
ATXQtyBase@ATXAT:NewLabel150QtyPreviousOprError��	TransDate@ATXAT:NewLabel151	TransDate��NoYes	NoYesIdReportedBySize�   � 

difference�  ATXQtyRemain� �� 
Percent�  Percent� �� 
validateField   � _fieldIdToCheck FieldId��  boolean� �� 	
fisrtOprNum   � _prodId ProdId��  OprNum� �!ATXProductionFloorControl9  �1 �� �	BranchIdx  0public class ATXBranchTable extends common
{
}Storage for branch catalog   �   �BranchId��Description�
AutoReport��   �BranchId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �BranchId��Description�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �	ATXBranchIdBranchId��	DescriptionDescription�ATXBranchFormDisplay   �    �BranchId�		BranchIdx�%@ATXApparelAndTextile_en_US:ATXL00023   � 	
find   � 	_branchId ATXBranchId�� false
_forUpdate boolean��  ATXBranchTable� �� 	
exist   � 	_branchId ATXBranchId��  boolean� �!ATXBranchTable$	BranchIdx9  �3BranchId4Description�� �OrderIdx:public class ATXRequestOrderUpdates extends common
{

}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �RequestOrderUpdateId�	@SYS35893Overview�   �	TransDateRequestOrderDate��	ATXRequestOrderIdRequestOrderId��ATXRequestOrderUpdateIdRequestOrderUpdateId�   �    �RequestOrderUpdateId�	OrderIdx�@ATXAT:NewLabel76   � 
initFromRequestOrderHeader   � _requestOrderHeader ATXRequestOrderHeader��  � �� 
ATXrequestOrderHeader�  ATXRequestOrderHeader� �� 	
find   � _requestOrderId ATXRequestOrderId�� _requestOrderUpdateId ATXRequestOrderUpdateId�� falseudpate boolean��  ATXRequestOrderUpdates� �� 	
lastVersion   � _requestOrderId ATXRequestOrderId��  ATXRequestOrderUpdateId� �!ATXRequestOrderUpdates%   �   �RequestOrderIdRequestOrderIdRequestOrderId�ATXRequestOrderHeaderATXRequestOrderHeader�9  ��� �ItemGridIdx2public class ATXItemGridTable extends common
{
}   �
AutoReport��   �
ItemGridId��
GridIdName��DimComboType�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �
ItemGridId��
GridIdName��DimComboType�	@SYS35893General�   �ATXDimComboTypeDimComboType��	Name
GridIdName��  	ATXItemGridId 
ItemGridId�ATXItemDimGrids   �    �
ItemGridId�	ItemGridIdx�@ATXAT:NewLabel66   � 
validateDelete�  boolean� �� 	
exist   � _itemGridId ATXItemGridId��  boolean� �� 	
existByType   � _itemGridId ATXItemGridId�� _type ATXDimComboType��  boolean� �� 	
find   � _itemGridId ATXItemGridId�� false_update boolean��  ATXItemGridTable� �� 	

findByType   � _itemGridId ATXItemGridId�� _type ATXDimComboType�� false_update boolean��  ATXItemGridTable� �� 
modifiedField   � _fieldId FieldId��  � �!ATXItemGridTable$ItemGridIdx9  �3
ItemGridId4
GridIdName�� ��+public class ATXProdCutPatternBreakdown extends common
{
    /*/// <summary>
    ///
    /// </summary>
    /// <param name = "breakDown"></param>
    public void initFromBreakdownOrderLine(BreakdownOrderLine_AT breakDown)
    {
        ProdCutPattern_AT pattern;

        if (breakDown)
        {
            select firstonly pattern
                where pattern.RecId == this.ProdCutPatternRecId;
            if (pattern)
            {
                this.InventSizeId = breakDown.InventSizeId;
                this.QtyOrig      = breakDown.Qty;
                this.CanvasQty    = this.BagQty * pattern.BagQty * pattern.CanvasQty;
            }
        }
    }

    /// <summary>
    ///
    /// </summary>
    /// <param name = "_fieldId"></param>
    public void modifiedField(FieldId _fieldId)
    {
        super(_fieldId);

        switch (_fieldId)
        {
            case fieldNum(ProdCutPatternBreakdown_AT, BagQty):
                this.calcQty();
                break;
        }
    }

    /// <summary>
    /// Update totals
    /// </summary>
    public void calcQty()
    {
        ProdCutPattern_AT prodCutPattern;

        prodCutPattern = ProdCutPattern_AT::find(this.ProdCutPatternRecId);
        this.CanvasQty = this.BagQty * prodCutPattern.CanvasQty * prodCutPattern.BagQty;
        this.CanvasSubtotalQty = ProdCutPatternBreakdown_AT::getCanvasSubtotalQty(this.ProdCutPatternRecId, this.InventSizeId);
        this.RemainCanvas = this.QtyOrig - this.CanvasSubtotalQty;
    }

    /// <summary>
    ///
    /// </summary>
    /// <param name = "_recId"></param>
    /// <returns></returns>
    public static Qty getCanvasSubtotalQty(RefRecId _recIdPattern, EcoResSizeName _size)
    {
        ProdCutPatternBreakdown_AT  prodCutPatternBreakdown;
        ProdCutPattern_AT           prodCutPattern, prodCutPatternOff;
        ProdCutSection_AT           prodCutSection;

        
        select sum(CanvasQty) from prodCutPatternBreakdown
            where prodCutPatternBreakdown.InventSizeId    == _size
            join prodCutPattern
            where prodCutPattern.recId               == prodCutPatternBreakdown.ProdCutPatternRecId
            join prodCutSection
            where prodCutSection.RecId == prodCutPattern.ProdCutSectionRecId
            && prodCutSection.ProdCutHeaderRecId == ProdCutSection_AT::find(ProdCutPattern_AT::find(_recIdPattern).ProdCutSectionRecId).ProdCutHeaderRecId;

        return prodCutPatternBreakdown.CanvasQty;
    }

    /// <summary>
    ///
    /// </summary>
    /// <param name = "_recId"></param>
    /// <returns></returns>
    public static Qty getBagTotalQty(RefRecId _recId)
    {
        ProdCutPatternBreakdown_AT prodCutPatternBreakdown;

        select sum(bagQty) from prodCutPatternBreakdown
            where prodCutPatternBreakdown.ProdCutPatternRecId == _recId;

        return prodCutPatternBreakdown.bagQty;
    }

    /// <summary>
    ///
    /// </summary>
    /// <param name = "_recId"></param>
    /// <returns></returns>
    public static Qty getCanvasQty(RefRecId _recId)
    {
        ProdCutPatternBreakdown_AT prodCutPatternBreakdown;

        select sum(CanvasQty) from prodCutPatternBreakdown
            where prodCutPatternBreakdown.ProdCutPatternRecId == _recId;

        return prodCutPatternBreakdown.CanvasQty;
    }

    /// <summary>
    ///
    /// </summary>
    public void update()
    {
        super();
        
        this.CanvasSubtotalQty = ProdCutPatternBreakdown_AT::getCanvasSubtotalQty(this.ProdCutPatternRecId,this.InventSizeId);
        this.RemainCanvas = this.QtyOrig - this.CanvasSubtotalQty;
    }

    /// <summary>
    /// Get Total for all sections
    /// </summary>
    /// <param name = "_recId"></param>
    /// <returns></returns>
    public static Qty getCanvasQtySection(RefRecId _recId)
    {
        ProdCutPatternBreakdown_AT prodCutPatternBreakdown;
        ProdCutPattern_AT prodCutPattern_AT;

        select sum(CanvasQty) from prodCutPatternBreakdown
            join prodCutPattern_AT
            where prodCutPattern_AT.RecId == prodCutPatternBreakdown.ProdCutPatternRecId
                && prodCutPattern_AT.ProdCutSectionRecId == _recId
        ;

        return prodCutPatternBreakdown.CanvasQty;
    }

    /// <summary>
    /// Get Marker qty from all sections
    /// </summary>
    /// <param name = "_recIdSection"></param>
    /// <returns></returns>
    public static Qty getCanvasQtyCutHeader(RefRecId _recIdSection)
    {
        ProdCutSection_AT prodCutSection_ATQry, prodCutSection_AT = ProdCutSection_AT::find(_recIdSection);
        ProdCutPatternBreakdown_AT prodCutPatternBreakdown;
        ProdCutPattern_AT prodCutPattern_AT;

        select sum(CanvasQty) from prodCutPatternBreakdown
            join prodCutPattern_AT
            where prodCutPattern_AT.RecId == prodCutPatternBreakdown.ProdCutPatternRecId
            join prodCutSection_ATQry
            where prodCutSection_ATQry.RecId == prodCutPattern_AT.ProdCutSectionRecId
                && prodCutSection_ATQry.ProdCutHeaderRecId == prodCutSection_AT.ProdCutHeaderRecId;

        return prodCutPatternBreakdown.CanvasQty;
    }

    /// <summary>
    ///
    /// </summary>
    public void insert()
    {
        this.RetailDisplayOrder = SizeDisplayOrder_AT::find(this.InventSizeId).RetailDisplayOrder;
        super();
    }*/

}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �InventSizeId��CutQty�	@SYS35893General�   �RefRecIdProdCutPatternRecId��    	EcoResSizeNameInventSizeId��	ATXCutQtyCutQty�   �    �ProdCutPatternRecId�	ProdCutPatterndx�@ATXAT:NewLabel288!ATXProdCutPatternBreakdown%   �    �ProdCutPatternRecIdProdCutPatternRecIdRecId�ATXProdCutPatternATXProdCutPattern�9  �3ProdCutPatternRecId4InventSizeId�� �ATXPLM7public class ATXProductPreProdTask extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �LineNumber_IT��PreProdTaskId��PlanDate��	TransDate��
AssignedTo��Approver��Approved�	@SYS35893General��   �SampleBookId��RequestOrderId��ItemId�	@SYS40441	Reference�   �	ItemIdItemId��  	ATXPreProdTaskId PreProdTaskId��	TransDate@ATXPLM:NewLabel8PlanDate��    	TransDate	TransDate��HcmWorkerRecId@ATXPLM:NewLabel5
AssignedTo��    HcmWorkerRecId@ATXPLM:NewLabel10Approver��    NoYes	ATXApprovedApproved��	ATXSampleBookIdSampleBookId��ATXPreProdTaskTypePreProdTaskType��	ATXRequestOrderIdRequestOrderId��LineNumber_ITLineNumber_IT�   �    �ItemId��RequestOrderId��LineNumber_IT�	LineNumberIdx�@ATXPLM:NewLabel7   � 	
existByRequest   � _requestOrderId ATXRequestOrderId��  boolean� �!ATXProductPreProdTask%   �   �PreProdTaskIdPreProdTaskIdPreProdTaskId�ATXPreProdTaskATXPreProdTask��   �
AssignedTo
AssignedToRecId�RecId		HcmWorker	HcmWorker��   �ApproverApproverRecId�RecId	
HcmWorker1	HcmWorker��   �SampleBookIdSampleBookIdSampleBookId�ATXSampleBookTableATXSampleBookTable�9  ��� �ItemIdx8public class ATXBOMBlockingLogTable extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ItemId��BOMId��	BOMTypeId��BOMTypeIdActive��Notes�	@SYS35893Overview�   �	ItemIdItemId��	BOMIdBOMId��	ATXBOMTypeId	BOMTypeId��NoYes	NoYesIdBOMTypeIdActive��	NotesNotes��DateTimeExecutedDateTimeUpdated�   �    �ItemId��BOMId��	BOMTypeId�	ItemIdx�@ATXAT:NewLabel71   � 	
find   � _itemId ItemId�� _bomTypeId_AT ATXBOMTypeId�� false
_forUpdate boolean��  ATXBOMBlockingLogTable� �� 	
findByBomId   � _itemId ItemId�� _bomTypeId_AT ATXBOMTypeId�� _bomId BOMId�� false
_forUpdate boolean��  ATXBOMBlockingLogTable� �� 
insert�  � �� 
update�  � �!ATXBOMBlockingLogTable$ItemIdx9  �3ItemId4BOMId�� �RequestOrderIdx8public class ATXRequestOrderRelease extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	ATXRequestOrderIdRequestOrderId��NoYes	NoYesIdGenerateRequestBOMBatch  ��	SalesIdSalesId�   �    �RequestOrderId�	RequestOrderIdx�@ATXAT:NewLabel69   � 	
find   � _requestOrderId_AT ATXRequestOrderId�� false
_forUpdate boolean��  ATXRequestOrderRelease� �!ATXRequestOrderRelease$RequestOrderIdx9  �3RequestOrderId�� �<public class ATXRouteCardBreakdownTmp extends common
{
}
   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	EcoResSizeNameInventSizeId��QtyQty�!ATXRouteCardBreakdownTmp9  �1 �� �6public class ATXCutTechnicalSheet extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �CutAccesoryItem��Fabric��	Placement��CutWidth��CutDirection��Supply��Notes�CutAccesories�   �	ItemIdItemId��	
RouteOprId
RouteOprId��	DescriptionAccesory��	Description@ATXPLM:NewLabel25Fabric��	Description@ATXPLM:NewLabel26	Placement��Qty@ATXPLM:NewLabel27CutWidth��	Description@ATXPLM:NewLabel28CutDirection��	Description@ATXPLM:NewLabel29Supply��	Description@ATXPLM:NewLabel22Notes��QtyTemp��QtyTime��QtyPressure��	DescriptionPressureUOM��	ItemId@ATXPLM:NewLabel24CutAccesoryItem�!ATXCutTechnicalSheet%   �   �ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �7public class ATXRejectionCodeTable extends common
{
}   �
AutoReport��   �RejectionCodeId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �RejectionCodeId��Description�Overview�   �	ATXRejectionCodeIdRejectionCodeId��	DescriptionDescription�ATXRejectionCodeTable   �   �RejectionCodeId�	RejectionCodeIdx�   � 	
find   � _rejectionCodeId ATXRejectionCodeId�� false_update boolean��  ATXRejectionCodeTable� �� 	
exist   � _rejectionCodeId ATXRejectionCodeId��  boolean� �!ATXRejectionCodeTable9  ��� �KeyIdx6public class ATXSalesParameters extends common
{

}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �NumberSequenceId��RequestOrderType��InventSiteId��InventLocationId��WMSLocationId�	@SYS35893Overview��   �ValidatePrice��GenerateRequestBOMBatch��WMSOrderForSales�@ATXAT:NewLabel9RequestOrder�
   �	InventSiteIdInventSiteId��	InventLocationIdInventLocationId��	WMSLocationIdWMSLocationId��ATXRequestOrderTypeRequestOrderType��RecId%@ATXApparelAndTextile_en_US:ATXL00131NumberSequenceId��NoYes	NoYesIdWMSOrderForSales��NoYes	NoYesId@ATXAT:NewLabel40ValidatePrice��NoYes	NoYesIdGenerateRequestBOMBatch��NoYes	NoYesIdSkipClosedSL��    ParametersKeyKey  �   �    �Key�	KeyIdx�@ATXAT:NewLabel84   � 	
find   � false
_forUpdate boolean��  ATXSalesParameters� �!ATXSalesParameters$KeyIdx%   �   �NumberSequenceIdNumberSequenceIdRecId�NumberSequenceTableNumberSequenceTable�9  �0 3Key�� �;public class ATXEventWarningParameters extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �RequestOrderReleaseGroup��RequestOrderReleaseSample��CustRefRequestOrderChanged��SizeOrQtyRequestOrderChanged��CreateItemWarningGroupId��ProdPoolIdExtraction��RequestOrderPlanTA�	@SYS35893Overview�   �	ATXWarningGroupId%@ATXApparelAndTextile_en_US:ATXL00051RequestOrderReleaseGroup��	ATXWarningGroupId%@ATXApparelAndTextile_en_US:ATXL00052CustRefRequestOrderChanged��	ATXWarningGroupId%@ATXApparelAndTextile_en_US:ATXL00053SizeOrQtyRequestOrderChanged��	ATXWarningGroupId%@ATXApparelAndTextile_en_US:ATXL00054RequestOrderReleaseSample��	ATXWarningGroupId%@ATXApparelAndTextile_en_US:ATXL00055CreateItemWarningGroupId��	
ProdPoolId%@ATXApparelAndTextile_en_US:ATXL00056ProdPoolIdExtraction��	ATXWarningGroupId%@ATXApparelAndTextile_en_US:ATXL00057RequestOrderPlanTA�@ATXAT:NewLabel79   � 	
find   � false
_forUpdate boolean��  ATXEventWarningParameters� �!ATXEventWarningParameters%   �   �RequestOrderReleaseGroupRequestOrderReleaseGroupWarningGroupId�ATXEventWarningsGroupATXEventWarningsGroup��   �SizeOrQtyRequestOrderChangedSizeOrQtyRequestOrderChangedWarningGroupId�EventWarningsGroupATXEventWarningsGroup��   �CustRefRequestOrderChangedCustRefRequestOrderChangedWarningGroupId�EventWarningsATXEventWarningsGroup��   �RequestOrderReleaseSampleRequestOrderReleaseSampleWarningGroupId�EventWarningsSamplesATXEventWarningsGroup��   �CreateItemWarningGroupIdCreateItemWarningGroupIdWarningGroupId�FabricWarningATXEventWarningsGroup��   �RequestOrderPlanTARequestOrderPlanTAWarningGroupId�EventWarningsTAATXEventWarningsGroup�9  ��� �1public class ATXSubOperation extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SubOperationId��Name�@ATXAT:NewLabel214General�   �	ATXSubOperationIdSubOperationId��	NameName�ATXSubOperation   �   �SubOperationId�	SubOperationIdx�@ATXAT:NewLabel304   � 	
find   � _subOperationId ATXSubOperationId�� false
_forUpdate boolean��  ATXSubOperation� �!ATXSubOperation9  �3SubOperationId4Name�� �=public class ATXProdQualityDimFieldSetUp extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �  FieldId DimensionFieldId	InventDim��  NoYes	NoYesId@ATXAT:NewLabel144IsActive��LineNum
LineNumber��RefRecIdProdQuality��	ATXAnyValueValue�   � 
	fieldName�  EcoResProductDimensionName� �� 
initFromProductDimensionGroup   � _ProdQualityTable ATXProdQualityTable��  � �� 
	initValue�  � �� 
validateDimensionsActive�  boolean� �� 	
findByDimensionGroupFieldId   � _productDimensionRecId RefRecId�� _dimensionFieldId  �� false_update boolean��  ATXProdQualityDimFieldSetUp� �!ATXProdQualityDimFieldSetUp%   �   �ProdQualityProdQualityRecId�ATXProdQualityTableATXProdQualityTable�9  ��� �ATXPLM8public class ATXPreProdTaskTemplate extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �PreProdTaskType��LineNumber_IT��PreProdTaskId��Days�	@SYS35893General�   �  ATXPreProdTaskTypePreProdTaskType��  	ATXPreProdTaskId PreProdTaskId��DaysDays��LineNumber_ITLineNumber_IT�   �    �PreProdTaskType��PreProdTaskId�	PreProdTaskIdx��    �PreProdTaskType��LineNumber_IT�	
LineNumIdx�@ATXPLM:NewLabel11!ATXPreProdTaskTemplate%   �   �PreProdTaskIdPreProdTaskIdPreProdTaskId�ATXPreProdTaskATXPreProdTask�9  �3PreProdTaskType4PreProdTaskId�� �6public class ATXItemCategoryTable extends common
{
}   �   �ItemCategoryId��Description�
AutoReport��   �ItemCategoryId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ItemCategoryId��Description�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �	ATXItemCategoryIdItemCategoryId��	DescriptionDescription�ATXItemCategoryTableForm   �    �ItemCategoryId�	CategoryIdx�%@ATXApparelAndTextile_en_US:ATXL00040   � 	
find   � 
_ctegoryId ATXItemCategoryId�� false_update boolean��  ATXItemCategoryTable� �� 	
exist   � 
_ctegoryId ATXItemCategoryId��  boolean� �� 
modifiedField   � _fieldId FieldId��  � �!ATXItemCategoryTable9  �3ItemCategoryId4Description�� �DestinationPlaceIdx5public class ATXDestinationPlace extends common
{
}   �   �DestinationPlaceId��Description�
AutoReport��   �DestinationPlaceId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �DestinationPlaceId��Description�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �  	ATXDestinationPlaceId DestinationPlaceId��	DescriptionDescription�ATXDestinationPlaceForm   �    �DestinationPlaceId�	DestinationPlaceIdx�@ATXAT:NewLabel87   � 	
find   � destinationPlaceId ATXDestinationPlaceId�� falseupdate boolean��  ATXDestinationPlace� �!ATXDestinationPlace9  �3DestinationPlaceId4Description�� �2public class ATXRouteOprTable extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �
RouteOprId��GetPreviousQty��SuggestWrkCtrId��ValidateCutId��BreakdownSize�Overview�   �NoYes	NoYesId@ATXAT:NewLabel238GetPreviousQty��NoYes	NoYesIdOEE��NoYes	ProdAutoPicklistProdAutoPicklist��	
RouteOprId
RouteOprId��NoYes	NoYesId@ATXAT:NewLabel237SuggestWrkCtrId��NoYes	NoYesId@ATXAT:NewLabel236BreakdownSize��NoYes	NoYesId@ATXAT:NewLabel235ValidateCutId�   �    �
RouteOprId�	OprIdx�   � 
oprName�  Name� �� 	
exist   � 
_operation 
RouteOprId��  boolean� �� 	
find   � 
_operation 
RouteOprId�� false
_forUpdate boolean��  ATXRouteOprTable� �!ATXRouteOprTable%   �   �
RouteOprId
RouteOprIdOprId�RouteOprTableRouteOprTable�9  ��� �:public class ATXCutTechnicalSheetWash extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��
   �CutAccesoryItem��ItemName��ClothGarment��SendBy��Sleeves��SpecialComponent��Service��WashType��
DyeingType��Combinations�Overview�   �	ItemIdItemId��	
RouteOprId
RouteOprId��	DescriptionAccesory��Qty@ATXPLM:NewLabel36InWidth��	Description@ATXPLM:NewLabel28CutDirection��	Description@ATXPLM:NewLabel29Supply��	Description@ATXPLM:NewLabel22Notes��Qty@ATXPLM:NewLabel32Temp��Qty@ATXPLM:NewLabel33Time��Qty@ATXPLM:NewLabel34Pressure��	Description@ATXPLM:NewLabel35PressureUOM��	ItemId@ATXPLM:NewLabel31CutAccesoryItem��	Description@ATXPLM:NewLabel38BendingType��	Description@ATXPLM:NewLabel26	Placement��	Description@ATXPLM:NewLabel21
SewMachine��Qty@ATXPLM:NewLabel37OutWidth��	Description@ATXPLM:NewLabel40ClothGarment��	Description@ATXPLM:NewLabel41SendBy��	Description@ATXPLM:NewLabel42Sleeves��	Description@ATXPLM:NewLabel43SpecialComponent��	Description@ATXPLM:NewLabel44Service��	Description@ATXPLM:NewLabel45WashType��	Description@ATXPLM:NewLabel46
DyeingType��	Description@ATXPLM:NewLabel47Combinations�   � 
ItemName�  ItemName� �!ATXCutTechnicalSheetWash%   �   �ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �"@DMF:StagingDeveloperDocumentation   � 
AutoReport�� 
AutoLookup��  AutoIdentification�� AutoSummary�� 
AutoBrowse��   �DefinitionGroup��
IsSelected��TransferStatus��ExecutionId� @DMF:StagingExtensionGroupExtensionList�   �  	DMFDefinitionGroupName  DefinitionGroup<   ��  	DMFExecutionId  ExecutionIdZ   ��NoYes	DMFIsSelected 
IsSelected��DMFTransferStatus TransferStatus��	InventSiteId InventSiteId��	InventLocationId InventLocationId��	WMSLocationId WMSLocationId��ATXRequestOrderType RequestOrderType��NoYes	NoYesId WMSOrderForSales��NoYes	NoYesId @ATXAT:NewLabel40ValidatePrice��NoYes	NoYesId GenerateRequestBOMBatch��NoYes	NoYesId SkipClosedSL��    ParametersKey Key�   �    �DefinitionGroup��ExecutionId��Key� 	
StagingIdx�@ATXAT:NewLabel84!ATXSalesParametersStaging$
StagingIdx%   �    �KeyKeyKey�(@DMF:StagingToDataEntityRelationshipRole 	
DataEntityATXSalesParametersEntity    �&
StagingIdx(  0 3Key�� �	 
 3public class ATXProdCutPattern extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �Marker��Section��MarkerMaking��MarkerSection��	CanvasQty��ProdQty�Overview�   �	String30@ATXAT:NewLabel185Marker��    	
ATXSectionSection��QtyBagQty��
ATXQtyBase@ATXAT:NewLabel290	CanvasQty��    Qty@ATXAT:NewLabel188ProdQty��    Qty@ATXAT:NewLabel189TotalBagQty��    Qty@ATXAT:NewLabel185SubtotalCanvasQty��    Qty@ATXAT:NewLabel190RemainCanvasQty��RefRecIdProdCutSectionRecId��Percent@ATXAT:NewLabel170YieldPercent��	ATXMarkerMakingMarkerMaking��	ATXMarkerSectionMarkerSection�   �    �ProdCutSectionRecId�	ProdCutSectionIdx�@ATXAT:NewLabel184   � 	
find   � _recId RefRecId��  ATXProdCutPattern� �� 
insert�  � �  !ATXProdCutPattern%   �   �ProdCutSectionRecIdProdCutSectionRecIdRecId�ATXProdCutSectionATXProdCutSection��   �RecIdRecIdRecId�ATXProdCutPatternATXProdCutPattern�9  ��� �KeyIdx6public class ATXProductParameters extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �AddScrapToSalesBOMQty��LockBOMTemplate��Key��
DummyValue�	@SYS35893General�   �NoYes	NoYesId%@ATXApparelAndTextile_en_US:ATXL00077LockBOMTemplate��    ParametersKeyKey  ��	SysGroup%@ATXApparelAndTextile_en_US:ATXL00080 
DummyValue��NoYes	NoYesId@ATXAT:NewLabel123AddScrapToSalesBOMQty�   �    �Key�	KeyIdx�@ATXAT:NewLabel10   � 	
find   � false
_forupdate boolean��  ATXProductParameters� �!ATXProductParameters$KeyIdx9  �0 3Key�� �KeyIdx@public class ATXApparelAndTextileParameters extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �Active�	@SYS35893General�   �    ParametersKeyKey  ��NoYes	NoYesId@ATXAT:NewLabel286Active�   �    �Key�	KeyIdx�@ATXAT:NewLabel2   � 	
find   � false
_forupdate boolean��  ATXApparelAndTextileParameters� �!ATXApparelAndTextileParameters$KeyIdx9  �0 3Key�� �7public class ATXRouteCardHeaderTmp extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	ProdIdProdId��	ItemIdItemId��	ItemNameItemName��	CustPurchaseOrderCustPurchaseOrder��	CustNameCustName��	SalesIdSalesId��	InventBatchIdInventBatchId��	ATXSeasonIdSeasonId��	ATXDestinationPlaceIdDestinationPlaceId��	TransDateDeliveryDate��	DescriptionProdIdBarcode�!ATXRouteCardHeaderTmp9  �1 �� �LineIdx;public class ATXLineOfBusinessBOMBatch extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	LineOfBusinessIdLineOfBusinessId�   �    �LineOfBusinessId�	LineIdx�@ATXAT:NewLabel22   � 	
find   � _lineOfBusinessId LineOfBusinessId�� false
_forUpdate boolean��  ATXLineOfBusinessBOMBatch� �!ATXLineOfBusinessBOMBatch$LineIdx9  �3
DataAreaId�� �3public class ATXPlacementTable extends common
{
}   �   �PlacementId��Description�
AutoReport��   �PlacementId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �PlacementId��Description�	@SYS35893Overview�   �	ATXPlacementIdPlacementId��	DescriptionDescription�ATXPlacementForm   �    �PlacementId�	PlacementIdx�@ATXAT:NewLabel51   � 	
find   � _placementId ATXPlacementId�� false
_forUpdate boolean��  ATXPlacementTable� �� 	
exist   � _placementId ATXPlacementId��  boolean� �!ATXPlacementTable9  ��� �SampleBookIdx	 
 4public class ATXSampleBookTable extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SampleBookId��SeasonId��CustAccount��BrandId��QuantityPlan��productsInSampleBook��	StartDate��EndDate�	@SYS35893General��   �SampleBookId�Id�   �  	ATXSampleBookId SampleBookId��	ATXSeasonIdSeasonId��	CustAccountCustAccount��	
ATXBrandIdBrandId��NumberOfRecords@ATXPLM:NewLabel15QuantityPlan��	StartDate	StartDate��EndDateEndDate�ATXSampleBook   �    �SampleBookId�	SampleBookIdx�@ATXPLM:NewLabel14   �     !SysClientCacheDataMethodAttribute     True��
productsInSampleBook�  NumberOfRecords� �  !ATXSampleBookTable$SampleBookIdx%   �   �SeasonIdSeasonIdSeasonId�ATXSeasonTableATXSeasonTable��   �BrandIdBrandIdBrandId�ATXBrandTableATXBrandTable�9  �3SampleBookId4SeasonId�� �;public class ATXCutTechnicalSheetApp extends common
{
}
   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �CutAccesoryItem��	Placement��
SewMachine��InWidth��OutWidth��CutDirection��BendingType��Notes�App�   �	ItemIdItemId��	
RouteOprId
RouteOprId��	DescriptionAccesory��Qty@ATXPLM:NewLabel36InWidth��	Description@ATXPLM:NewLabel28CutDirection��	Description@ATXPLM:NewLabel29Supply��	Description@ATXPLM:NewLabel22Notes��Qty@ATXPLM:NewLabel32Temp��Qty@ATXPLM:NewLabel33Time��Qty@ATXPLM:NewLabel34Pressure��	Description@ATXPLM:NewLabel35PressureUOM��	ItemId@ATXPLM:NewLabel31CutAccesoryItem��	Description@ATXPLM:NewLabel38BendingType��	Description@ATXPLM:NewLabel26	Placement��	Description@ATXPLM:NewLabel21
SewMachine��Qty@ATXPLM:NewLabel37OutWidth�!ATXCutTechnicalSheetApp%   �   �ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �
ProdCutIdx	 
 3public class ATXProdCutSection extends common
{
}   �
AutoReport��   �CutId��Prodid��CutQty�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��
   �CutId��InventItemPatternId��Section��WrkCtrId��CutQty��Locked��ReleasedDate��PrintBagCtrl��Finished��FinishedDate�Overview��   �ProdId��NumberOfPatterns�General�   �	ProdIdProdId��	ATXCutIdCutId��	ATXInventItemPatternIdInventItemPatternId��	
ATXSectionSection��    NoYes	NoYesId@ATXAT:NewLabel167Locked��	WrkCtrId@ATXAT:NewLabel168WrkCtrId��QtyQty��ATXYieldAvg@ATXAT:NewLabel170YieldQty��Qty@ATXAT:NewLabel171PocketingQty��	Notes@ATXAT:NewLabel172MarkerComments��	Notes@ATXAT:NewLabel173SectionComments��RefRecIdProdCutHeaderRecId��
ATXQtyBase@ATXAT:NewLabel174Units��	Description@ATXAT:NewLabel175	FoleoType��Qty@ATXAT:NewLabel176YDSRT��ATXYieldAvg@ATXAT:NewLabel177YieldQtyOverPct��  ATXReleasedDateReleasedDate��  	ATXCutQtyCutQty��    NumberOf@ATXAT:NewLabel179NumberOfPatterns��  NoYes	NoYesId@ATXAT:NewLabel180PrintBagCtrl��    ATXYieldAvg@ATXAT:NewLabel170YieldQtyAvg��  NoYes	NoYesId@ATXAT:NewLabel181Finished��  	TransDate@ATXAT:NewLabel182FinishedDate�   �    �ProdId��CutId�	
ProdCutIdx�	   � 
iniFromProdCutHeader   � _prodCutHeader ATXProdCutHeader��  � �� 
setYieldNewSection�  � �� 	
	nextCutId�   � �� 	
find   � _recIdSection RefRecId�� false
_forUpdate boolean��  ATXProdCutSection� �� 	
	findCutId   � _cutId ATXCutId�� false
_forUpdate boolean��  ATXProdCutSection� �� 
modifiedField   � _fieldId FieldId��  � �� 
ATXProdCutHeader�  ATXProdCutHeader� �� 
aosValidateDelete�  boolean� �� 	
exist   � _cutId ATXCutId��  boolean� �  !ATXProdCutSection%   �    �ProdCutHeaderRecIdProdCutHeaderRecIdRecId�ATXProdCutHeaderATXProdCutHeader  ��   �WrkCtrIdWrkCtrIdWrkCtrId�WrkCtrTableWrkCtrTable�9  �0 �� �KeyIdx3public class ATXProdParameters extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �CreateBOMStyles��ReqCalcScheduleItem��BOMVersionApproved��BOMRouteApprover�@ATXAT:NewLabel9Request��   �YieldPercent�@ATXAT:NewLabel213Yield��   �ValidateQtyOnPreviousOperation��ValidateEmplId��ValidateQuality�@ATXAT:NewLabel212FloorControlValidations��   �SuggestPersonnelNumber��ValidateGoodErrorQty��ATXProdCutNumberSequenceId��StopProdJournalDescription��JournalMovDescription�@ATXAT:NewLabel207	ShopFloor��   �ActivateCutControls��StandarPack��ExistenceInLastOperation�@ATXAT:NewLabel214Overview��   �LastOperationJournalName��ReverseInvMovJournalName�@ATXAT:NewLabel267LastRouteOpr�   �ParametersKeyKey��NoYes	NoYesId@ATXAT:NewLabel13@ATXAT:NewLabel12CreateBOMStyles��NoYes	NoYesId@ATXAT:NewLabel124BOMVersionApproved��BOMRouteApprover@ATXAT:NewLabel125BOMRouteApprover��NoYes	NoYesId@ATXAT:NewLabel122ReqCalcScheduleItem��NoYes	NoYesId@ATXAT:NewLabel152ValidateQtyOnPreviousOperation��NoYes	NoYesId@ATXAT:NewLabel153ValidateGoodErrorQty��Percent@ATXAT:NewLabel177YieldPercent��NoYes	NoYesId@ATXAT:NewLabel206ActivateCutControls��NoYes	NoYesId@ATXAT:NewLabel233SuggestPersonnelNumber��QtyStandarPack��	NumberSequenceCodeATXProdCutNumberSequenceId��	Description@ATXAT:NewLabel249StopProdJournalDescription��NoYes	NoYesId@ATXAT:NewLabel250ExistenceInLastOperation��NoYes	NoYesId@ATXAT:NewLabel251ValidateEmplId��NoYes	NoYesId@ATXAT:NewLabel263ValidateQuality��	Description@ATXAT:NewLabel266LastOperationJournalName��	Description@ATXAT:NewLabel269ReverseInvMovJournalName��	Description@ATXAT:NewLabel272JournalMovDescription�   �    �Key�	KeyIdx�@ATXAT:NewLabel8   � 	
find   � false
_forupdate boolean��  ATXProdParameters� �!ATXProdParameters$KeyIdx%   �   �BOMRouteApproverBOMRouteApproverRecId�RecId		HcmWorker	HcmWorker�9  �0 3Key�� �BrandIdx/public class ATXBrandTable extends common
{
}   �   �BrandId��Description�
AutoReport��   �BrandId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �BrandId��Description�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �	
ATXBrandIdBrandId��	DescriptionDescription�ATXBrandTable   �    �BrandId�	BrandIdx�@ATXAT:NewLabel68!ATXBrandTable$BrandIdx9  �3BrandId4Description�� �ItemGridValueIdx2public class ATXItemGridLines extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ItemGridValue��Description��RetailDisplayOrder�	@SYS35893Overview�   �NoYes	NoYesIdCheck��	DescriptionDescription��  	ATXItemGridId 
ItemGridId��  	ATXItemGridValue ItemGridValue��RetailDisplayOrderRetailDisplayOrder�   �    �
ItemGridId��ItemGridValue�	ItemGridValueIdx�@ATXAT:NewLabel67   � 	
exist   � _itemGridId ATXItemGridId�� 
_gridValue ATXItemGridValue��  boolean� �� 	
find   � _itemGirdId ATXItemGridId�� 
_gridValue ATXItemGridValue�� false_update boolean��  ATXItemGridLines� �� 
modifiedField   � _fieldId FieldId��  � �!ATXItemGridLines$ItemGridValueIdx%   �   �
ItemGridId
ItemGridId
ItemGridId�ATXItemGridTableATXItemGridTable�9  �3
ItemGridId4ItemGridValue�� �ProdPoolIdx2public class ATXProdPoolSetup extends common
{
}   �
AutoReport��   �
ProdPoolId��InventSiteId�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �InventSiteId��
ProdPoolId��GroupByConfigId��GroupByInventColorId��GroupByInventSizeId��GroupByInventStyleId�	@SYS35893Overview�   �NoYes	NoYesId@ATXAT:NewLabel138GroupByConfigId��NoYes	NoYesId@ATXAT:NewLabel139GroupByInventColorId��NoYes	NoYesId@ATXAT:NewLabel140GroupByInventSizeId��NoYes	NoYesId@ATXAT:NewLabel141GroupByInventStyleId��	InventSiteIdInventSiteId��	
ProdPoolId
ProdPoolId�   �    �
ProdPoolId�	ProdPoolIdx�@ATXAT:NewLabel137   � 	
find   � _inventSiteId InventSiteId�� _prodPoolId 
ProdPoolId�� false
_forUpdate boolean��  ATXProdPoolSetup� �!ATXProdPoolSetup$ProdPoolIdx%   �   �InventSiteIdInventSiteIdSiteId�
InventSite
InventSite��   �
ProdPoolId
ProdPoolId
ProdPoolId�ProdPoolProdPool�9  ��� �RequestOrderIdx	 
 7public class ATXRequestOrderHeader extends common
{
}=This table is used to build the request orders header process   �   �RequestOrderId��RequestOrderType��RequestOrderStatus��SeasonId��RequestOrderDate��RequestOrderCancelDate��ReviewedOrderDate��BranchId��RequestOrderGroupId��ItemDivisionId��CustAccount��CurrencyCode��CustPurchaseOrder��CustRef��
ProdPoolId��SalesDlvTermId��	DlvModeId��SalesId��InventSiteId��InventLocationId�
AutoReport��   �RequestOrderId��RequestOrderType��RequestOrderStatus��SeasonId��RequestOrderDate�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �RequestOrderId��RequestOrderType��RequestOrderStatus��SalesId��CustAccount��LineOfBusinessId��CustPurchaseOrder��CustRef��
ProdPoolId��SeasonId��SampleTypeId��AuthDate��RequestOrderDate��RequestOrderCancelDate��ItemId��QtyOv�@ATXAT:NewLabel94Overview��	   �CustAccount��CurrencyCode��CustPurchaseOrder��CustRef��	DlvModeId��SalesDlvTermId��ItemDivisionId��Comments��SkipBOMValidation�@ATXAT:NewLabel92	CustGroup��   �RequestOrderDate��RequestOrderCancelDate��ReviewedOrderDate�@ATXAT:NewLabel91
DatesGroup��   �InventSiteId��InventLocationId�@ATXAT:NewLabel93InventDimGroup��   �SeasonId��BranchId��RequestOrderGroupId��
ProdPoolId��DestinationPlaceId��SampleTypeId�@ATXAT:NewLabel98FilterGroup��%@ATXApparelAndTextile_en_US:ATXL00039ItemsDetails�,   �  	DescriptionCO��		String255%@ATXApparelAndTextile_en_US:ATXL00002Comments��	String10%@ATXApparelAndTextile_en_US:ATXL00003CPO��	CurrencyCodeCurrencyCode��	CustAccountCustAccount��	ATXCustClassIdCustClassId��  	CustPurchaseOrderCustPurchaseOrder��	CustRefCustRef��		DlvModeId	DlvModeId��NoYes	NoYesIdFiniched��	InventLocationIdInventLocationId��	InventSiteIdInventSiteId��	InventTransRefIdInventTransRefId��InventTransTypeInventTransType��	DescriptionPPK��	
ProdPoolId
ProdPoolId��	TransDate%@ATXApparelAndTextile_en_US:ATXL00005RequestOrderCancelDate��	TransDateRequestOrderCreated��ATXRequestOrderDateRequestOrderDate��	ATXRequestOrderGroupIdRequestOrderGroupId��  	ATXRequestOrderId RequestOrderId��    ATXRequestOrderStatusRequestOrderStatus��ATXRequestOrderTypeRequestOrderType��	TransDate%@ATXApparelAndTextile_en_US:ATXL00021ReviewedOrderDate��	SalesDlvTermIdSalesDlvTermId��	ATXSeasonIdSeasonId��	ATXBranchIdBranchId��	ATXItemDivisionIdItemDivisionId��    	SalesIdSalesId��	TransDateShipmentOrderDate��	DescriptionUPC��	ATXDestinationPlaceIdDestinationPlaceId��	ATXSampleTypeIdSampleTypeId��	TransDate%@ATXApparelAndTextile_en_US:ATXL00028AuthDate��	CustRef%@ATXApparelAndTextile_en_US:ATXL00029
CustRefOld��	ATXRequestOrderId%@ATXApparelAndTextile_en_US:ATXL00030PreviousRequestOrderId��	LineOfBusinessIdLineOfBusinessId��ATXIssueDate	IssueDate��	ATXCustPlanNumber
PlanNumber��	ProdId
ProdIdLink��	ItemIdItemId��Qty%@ATXApparelAndTextile_en_US:ATXL00033QtyOv��NoYes	NoYesId%@ATXApparelAndTextile_en_US:ATXL00034SkipBOMValidation��	ATXCustPlanNumberCustPlanNumber�ATXRequestOrder   �    �RequestOrderId�	RequestOrderIdx��    �CustAccount��CustPurchaseOrder�	CustAccountIdx��    �SalesId�	SalesIdx�@ATXAT:NewLabel4   � 
custName�  Name� �� 
displayCustRef�  Description255� �� 
jumpRefReferenceId�  boolean� �� 
modifiedField   � _fieldId FieldId��  � �� 
update�  � �� 
updateCustPurchaseOrder�  � �� 
updateRequestOrderCancelDate�  � �� 
updateRequestOrderDate�  � �� 
updateReviewedOrderDate�  � �� 
validateDelete�  boolean� �� 	
findByPurchaseOrder   � _custAccount CustAccount�� _custPurhaseOrder CustPurchaseOrder�� _requestOrderType ATXRequestOrderType�� false
_forUpdate boolean��  ATXRequestOrderHeader� �� 	
findBySalesId   � _salesId SalesId�� false
_forUpdate boolean��  ATXRequestOrderHeader� �� 	
findByPurchaseOrderCO   � _custAccount CustAccount�� _custPurhaseOrder CustPurchaseOrder�� _requestOrderType ATXRequestOrderType�� _co description�� false
_forUpdate boolean��  ATXRequestOrderHeader� �� 
	initValue�  � �� 	
find   � _requestOrderId ATXRequestOrderId�� false
_forUpdate boolean��  ATXRequestOrderHeader� �� 	
exist   � _requestOrderId ATXRequestOrderId��  boolean� �� 	
validatePODuplicated   � _custPurchaseOrder CustPurchaseOrder��  boolean� �  !ATXRequestOrderHeader$RequestOrderIdx%   �   �BranchIdBranchIdBranchId�ATXBranchTableATXBranchTable��   �ItemDivisionIdItemDivisionIdItemDivisionId�ATXItemDivisionTableATXItemDivisionTable��   �RequestOrderGroupIdRequestOrderGroupIdRequestOrderGroupId�ATXRequestOrderGroupTableATXRequestOrderGroupTable��   �SeasonIdSeasonIdSeasonId�ATXSeasonTableATXSeasonTable��   �CustAccountCustAccount
AccountNum�	CustTable	CustTable��   �
ProdPoolId
ProdPoolId
ProdPoolId�ProdPoolProdPool��   �	DlvModeId	DlvModeIdCode�DlvModeDlvMode��   �SalesIdSalesIdSalesId�
SalesTable
SalesTable��   �InventSiteIdInventSiteIdSiteId�
InventSite
InventSite��   �InventLocationIdInventLocationIdInventLocationId�InventlocationInventLocation��   �CurrencyCodeCurrencyCodeCurrencyCode�CurrencyCurrency��   �DestinationPlaceIdDestinationPlaceIdDestinationPlaceId�ATXDestinationPlaceATXDestinationPlace��   �SampleTypeIdSampleTypeIdSampleTypeId�ATXSampleTypeTableATXSampleTypeTable��   �RequestOrderIdRequestOrderIdRequestOrderId�ATXRequestOrderHeaderATXRequestOrderHeader�9  �3RequestOrderId�� �"@DMF:StagingDeveloperDocumentation   � 
AutoReport�� 
AutoLookup��  AutoIdentification�� AutoSummary�� 
AutoBrowse��   �DefinitionGroup��
IsSelected��TransferStatus��ExecutionId� @DMF:StagingExtensionGroupExtensionList�   �  	DMFDefinitionGroupName  DefinitionGroup<   ��  	DMFExecutionId  ExecutionIdZ   ��NoYes	DMFIsSelected 
IsSelected��DMFTransferStatus TransferStatus��NoYes	NoYesId %@ATXApparelAndTextile_en_US:ATXL00077LockBOMTemplate��    ParametersKey Key��	SysGroup %@ATXApparelAndTextile_en_US:ATXL00080 
DummyValue��NoYes	NoYesId @ATXAT:NewLabel123AddScrapToSalesBOMQty�   �    �DefinitionGroup��ExecutionId��Key� 	
StagingIdx�@ATXAT:NewLabel10!ATXProductParametersStaging$
StagingIdx%   �    �KeyKeyKey�(@DMF:StagingToDataEntityRelationshipRole 	
DataEntityATXProductParametersEntity    �&
StagingIdx(  0 3Key�� �4public class ATXBOMTemplateLine extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �MatrixConfig��ItemId��itemName��	nameAlias��	BOMTypeId��Blocking��PlacementId��OprNum��
RouteOprId��BOMQty��BOMQtySerie��UnitId��
ScrapConst��ScrapVar��ConfigIdFlag��InventSizeIdFlag��InventColorIdFlag��InventStyleIdFlag��BOMConsumpType��BOMType�	@SYS35893General��   �ConfigId��InventSizeId��InventColorId��InventStyleId�@ATXAT:NewLabel54ProductMasterDim��   �ConfigIdFlag��InventSizeIdFlag��InventColorIdFlag��InventStyleIdFlag�@ATXAT:NewLabel60GenerateBOMBy�-   �BOMConsumpTypeBOMConsumpType��	BOMIdBOMId��BOMQtyBOMQty��BOMQtySerieBOMQtySerie��BOMTypeBOMType��NoYes	BOMCalcBOMLineCalculation��	ConfigGroupIdConfigGroupId��NoYes	EcoResConfigurationFlagConfigIdFlag��NoYes	BOMEndSchedConsumpBOMEndSchedConsump��
BOMFormulaFormula��	StartDateFromDate��NoYes	NoYesIdHasAnyChild��	EcoResColorName@ATXAT:NewLabel57InventColorId��NoYes	EcoResColorFlagInventColorIdFlag��	InventDimIdInventDimId��	EcoResSizeName@ATXAT:NewLabel56InventSizeId��NoYes	EcoResSizeFlagInventSizeIdFlag��NoYes	EcoResStyleFlagInventStyleIdFlag��	ItemIdItemId��		ItemBOMId	ItemBOMId��	ItemRouteIdItemRouteId��	EcoResStyleName@ATXAT:NewLabel58InventStyleId��LineNumLineNum��NoYes	NoYesId
MainFabric��	SysGroupMaterialRouting��NoYes	NoYesId@ATXAT:NewLabel50@ATXAT:NewLabel59MatrixConfig��	String20MatrixId��OprNumBOMLineOprNum��OprNumBOMLineOprNumBOMLine��	BOMPositionPosition��ProdFlushingPrincipBOMProdFlushingPrincip��	InventLocationIdInventLocationId��	EcoResConfigurationName@ATXAT:NewLabel55ConfigId��	ATXPlacementIdPlacementId��	
RouteOprId
RouteOprId��		BOMUnitId	BOMUnitId��	VendAccountVendAccount��	ItemId@ATXAT:NewLabel276ProductMasterItemId��		BOMUnitIdUnitId��
ScrapConst
ScrapConst��ScrapVarScrapVar��	VendAccountVendId��boolean	WrkCtrConsumptionWrkCtrConsumption��NoYes	NoYesId@ATXAT:NewLabel52Blocking��	ATXBOMTypeId	BOMTypeId�   �    �BOMId��ItemId�	BOMIdx�@ATXAT:NewLabel22   � 	
	findRecId   � _recId RefRecId�� false
_forUpdate boolean��  ATXBOMTemplateLine� �� 	

existRecId   � _recId RefRecId��  boolean� ��     !SysClientCacheDataMethodAttribute     True��
	nameAlias�  	NameAlias� �� 
modifiedField   � _fieldId fieldId��  � ��     !SysClientCacheDataMethodAttribute     True��
itemName�  ItemName� �� 
inventTableBOMVersion�  InventTable� �� 
inventTable   � false
_forUpdate boolean��  InventTable� �� 
	inventDim   � false
_forUpdate boolean��  	InventDim� ��     !SysClientCacheDataMethodAttribute     True��
firstExternalItemId�  ExternalItemId� �� 
bomTable   � false
_forUpdate boolean��  BOMTable� �� 
validateDelete�  boolean� ��     !SysClientCacheDataMethodAttribute     True��
displayNameAlias�  	NameAlias� �� 
insert�  � �� 
	initValue�  � �!ATXBOMTemplateLine%   �   �BOMIdBOMIdBOMId��ProductMasterItemIdProductMasterItemIdItemId�
BOMVersion
BOMVersion��   �InventDimIdInventDimIdinventDimId�	InventDim	InventDim��   �ItemIdItemIdItemId�InventTableInventTable��   �	BOMTypeId	BOMTypeId	BOMTypeId�ATXBOMTypeTableATXBOMTypeTable�9  ��� �6public class ATXInventItemPattern extends common
{
}   �
AutoReport��   �InventItemPatternId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �InventItemPatternId��Description�Overview�   �	ATXInventItemPatternIdInventItemPatternId��	DescriptionDescription�ATXInventItemPattern   �   �InventItemPatternId�	InventItemPatternIdx�   � 	
find   � _inventItemPatternId ATXInventItemPatternId�� false
_forUpdate boolean��  ATXInventItemPattern� �� 	
exist   � _inventItemPatternId ATXInventItemPatternId��  boolean� �!ATXInventItemPattern9  ��� �BOMTemplateIdx8public class ATXBOMMatrixTemplate extends common
{

}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SeasonId��DestinationPlaceId��RequestOrderId��ProductMasterConfigId��ProductMasterInventSizeId��ProductMasterInventColorId��ProductMasterInventStyleId��SameProductMasterSize��ItemId��ConfigId��InventSizeId��InventColorId��InventStyleId��BOMQty��BOMQtySerie��BOMType��
RouteOprId��VendAccount�	@SYS35893General�   �BOMQtyBOMQty��BOMQtySerieBOMQtySerie��RefRecIdBOMTemplateLine��BOMTypeBOMType��	ItemIdItemId��	
RouteOprId
RouteOprId��	VendAccountVendAccount��	EcoResConfigurationName@ATXAT:NewLabel277ConfigId��	EcoResSizeName@ATXAT:NewLabel278InventSizeId��	EcoResColorName@ATXAT:NewLabel279InventColorId��	EcoResStyleName@ATXAT:NewLabel280InventStyleId��	EcoResConfigurationName@ATXAT:NewLabel55ProductMasterConfigId��	EcoResSizeName@ATXAT:NewLabel56ProductMasterInventSizeId��	EcoResColorName@ATXAT:NewLabel57ProductMasterInventColorId��	EcoResStyleName@ATXAT:NewLabel58ProductMasterInventStyleId��	ATXDestinationPlaceIdDestinationPlaceId��	ATXSeasonIdSeasonId��	ATXRequestOrderIdRequestOrderId��NoYes	NoYesId@ATXAT:NewLabel62SameProductMasterColor��NoYes	NoYesId@ATXAT:NewLabel61SameProductMasterSize��	ItemId@ATXAT:NewLabel276ProductMasterItemId�   �    �BOMTemplateLine�	BOMTemplateIdx�@ATXAT:NewLabel63   � 
inventTable�  InventTable� �� 
validateWrite�  boolean� �� 
bomTemplateLine�  ATXBOMTemplateLine� �!ATXBOMMatrixTemplate%   �   �BOMTemplateLineBOMTemplateLineRecId�ATXBOMTemplateLineATXBOMTemplateLine��   �SeasonIdSeasonIdSeasonId�ATXSeasonTableATXSeasonTable��   �DestinationPlaceIdDestinationPlaceIdDestinationPlaceId�ATXDestinationPlaceATXDestinationPlace��   �RequestOrderIdRequestOrderIdRequestOrderId�ATXRequestOrderHeaderATXRequestOrderHeader�9  �3ItemId�� �"@DMF:StagingDeveloperDocumentation   � 
AutoReport�� 
AutoLookup��  AutoIdentification�� AutoSummary�� 
AutoBrowse��   �DefinitionGroup��
IsSelected��TransferStatus��ExecutionId� @DMF:StagingExtensionGroupExtensionList�0   �  	DMFDefinitionGroupName  DefinitionGroup<   ��  	DMFExecutionId  ExecutionIdZ   ��NoYes	DMFIsSelected 
IsSelected��DMFTransferStatus TransferStatus��  	Description CO��		String255 %@ATXApparelAndTextile_en_US:ATXL00002Comments��	String10 %@ATXApparelAndTextile_en_US:ATXL00003CPO��	CurrencyCode CurrencyCode��	CustAccount CustAccount��	ATXCustClassId CustClassId��  	CustPurchaseOrder CustPurchaseOrder��	CustRef CustRef��		DlvModeId 	DlvModeId��NoYes	NoYesId Finiched��	InventLocationId InventLocationId��	InventSiteId InventSiteId��	InventTransRefId InventTransRefId��InventTransType InventTransType��	Description PPK��	
ProdPoolId 
ProdPoolId��	TransDate %@ATXApparelAndTextile_en_US:ATXL00005RequestOrderCancelDate��	TransDate RequestOrderCreated��ATXRequestOrderDate RequestOrderDate��	ATXRequestOrderGroupId RequestOrderGroupId��  	ATXRequestOrderId  RequestOrderId��    ATXRequestOrderStatus RequestOrderStatus��ATXRequestOrderType RequestOrderType��	TransDate %@ATXApparelAndTextile_en_US:ATXL00021ReviewedOrderDate��	SalesDlvTermId SalesDlvTermId��	ATXSeasonId SeasonId��	ATXBranchId BranchId��	ATXItemDivisionId ItemDivisionId��    	SalesId SalesId��	TransDate ShipmentOrderDate��	Description UPC��	ATXDestinationPlaceId DestinationPlaceId��	ATXSampleTypeId SampleTypeId��	TransDate %@ATXApparelAndTextile_en_US:ATXL00028AuthDate��	CustRef %@ATXApparelAndTextile_en_US:ATXL00029
CustRefOld��	ATXRequestOrderId %@ATXApparelAndTextile_en_US:ATXL00030PreviousRequestOrderId��	LineOfBusinessId LineOfBusinessId��ATXIssueDate 	IssueDate��	ATXCustPlanNumber 
PlanNumber��	ProdId 
ProdIdLink��	ItemId ItemId��Qty %@ATXApparelAndTextile_en_US:ATXL00033QtyOv��NoYes	NoYesId %@ATXApparelAndTextile_en_US:ATXL00034SkipBOMValidation��	ATXCustPlanNumber CustPlanNumber�ATXRequestOrder   �    �DefinitionGroup��ExecutionId��RequestOrderId� 	
StagingIdx�@ATXAT:NewLabel4! ATXRequestOrderHeaderDataStaging$
StagingIdx%   �    �RequestOrderIdRequestOrderIdRequestOrderId�(@DMF:StagingToDataEntityRelationshipRole 	
DataEntityATXRequestOrderHeaderDataEntity    �&
StagingIdx(  0 3RequestOrderId�� �Cpublic class ATXCutTechnicalSheetInterlining extends common
{
}
   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �CutAccesoryItem��Description��	Placement��CutWidth��CutDirection��Supply��Notes��Temp��Time��Pressure��PressureUOM�Interlining�   �	ItemIdItemId��	
RouteOprId
RouteOprId��	DescriptionAccesory��Qty@ATXPLM:NewLabel27CutWidth��	Description@ATXPLM:NewLabel28CutDirection��	Description@ATXPLM:NewLabel29Supply��	Description@ATXPLM:NewLabel22Notes��Qty@ATXPLM:NewLabel32Temp��Qty@ATXPLM:NewLabel33Time��Qty@ATXPLM:NewLabel34Pressure��	Description@ATXPLM:NewLabel35PressureUOM��	ItemId@ATXPLM:NewLabel31CutAccesoryItem��	DescriptionDescription��	Description@ATXPLM:NewLabel26	Placement�!ATXCutTechnicalSheetInterlining%   �   �ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �6public class ATXRequestOrderUsers extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �		SysUserIdUserId�@ATXAT:NewLabel81   � 	
find   � _userId UserId�� false
_forUpdate boolean��  ATXRequestOrderUsers� �!ATXRequestOrderUsers9  ��� �ProdIdx2public class ATXProdCutHeader extends common
{
}   � DeleteAction1 ATXProdCutSection �   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ProdId��CustAccount��ItemId��ItemName��CustPurchaseOrder��CustRef��EcoResColorName��RequestedDate��Qty��
QtyCutPlan��	QtyCutBag��ColorDescription��	Spreading�Overview�   �  	ProdId ProdId��    	CustPurchaseOrderCustPurchaseOrder��    	CustRefCustRef��    	CustAccountCustAccount��ATXRequestOrderDateRequestedDate��    
ATXQtyOrigQty��    	ItemIdItemId��    	ItemNameItemName��    	EcoResColorNameEcoResColorName��    	Description@ATXAT:NewLabel158ColorDescription��	ATXSpreading	Spreading��
ATXQtyBase@ATXAT:NewLabel160
QtyCutPlan��
ATXQtyBase@ATXAT:NewLabel161	QtyCutBag�   �   �ProdId�	ProdIdx�   � 	
find   � _prodId ProdId�� false
_forUpdate boolean��  ATXProdCutHeader� �� 
initFromProdTable   � 
_prodTable 	ProdTable��  � �� 	
	findRecId   � _recId RecId�� true
_forUpdate boolean��  ATXProdCutHeader� �!ATXProdCutHeader$ProdIdx%   �   �	Spreading	Spreading	Spreading�ATXSpreadingTableATXSpreadingTable��   �ProdIdProdIdProdId�	ProdTable	ProdTable�9  ��� �ReferenceIdx	 
 2public class ATXEmailWarnings extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �	Reference��
DatePosted��
Recipients��Subject��Message��Send��
FlowUpdate��CreatedDateTime��LineText��CustPurchaseOrder��CustRef�	@SYS35893Warnings�   �
RefTableId
RefTableId��RefRecIdRefRecId��		String255Subject��	NotesMessage��	Description	Reference��	TransDate
DatePosted��	Notes
Recipients��NoYes	NoYesIdSend��Integer
FlowUpdate��	ATXRequestOrderIdRequestOrderId��	CustPurchaseOrderCustPurchaseOrder��	CustRefCustRef��	LineOfBusinessIdLineOfBusinessId��	LinetextLineText��BlobdataFile�   �    �	Reference��
DatePosted��Send�	ReferenceIdx�@ATXAT:NewLabel73   � 	
sendMailCreateItem   � _inventTable InventTable��  � �� 	
sendMailBOMBlokingLog   � _bomBlockingLogTable ATXBOMBlockingLogTable��  � �� 
insert�  � �� 
initFromRequestOrderHeader   � _requestOrderHeader_AT ATXRequestOrderHeader��  � �!ATXEmailWarnings$ReferenceIdx9  �3Message�� �RequestOrderGroupIdx  ;public class ATXRequestOrderGroupTable extends common
{
}Storage for order group catalog   �   �RequestOrderGroupId��Description�
AutoReport��   �RequestOrderGroupId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �RequestOrderGroupId��Description�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �  	ATXRequestOrderGroupId RequestOrderGroupId��	DescriptionDescription�ATXRequestOrderGroupFormDisplay   �    �RequestOrderGroupId�	RequestOrderGroupIdx�%@ATXApparelAndTextile_en_US:ATXL00007   � 	
find   � _requestOrderGroupId ATXRequestOrderGroupId�� false
_forUpdate boolean��  ATXRequestOrderGroupTable� �� 	
exis   � _requestOrderGroupId ATXRequestOrderGroupId��  boolean� �!ATXRequestOrderGroupTable$RequestOrderGroupIdx9  �3RequestOrderGroupId4Description�� �	 
 2public class ATXSamplingPhase extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SamplingPhaseId�%@ATXApparelAndTextile_en_US:ATXL00009General�   �  	ATXSamplingPhaseId SamplingPhaseId�ATXSamplingPhase   �   �SamplingPhaseId�	SamplingPhaseIdx�@ATXPLM:NewLabel3  !ATXSamplingPhase$SamplingPhaseIdx9  �3SamplingPhaseId�� �
BOMTypeIdx1public class ATXBOMTypeTable extends common
{
}   �
AutoReport��   �	BOMTypeId��Description��ValidateRequest��GenerateProdBOM�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	ATXBOMTypeId	BOMTypeId��	DescriptionDescription��NoYes	NoYesIdValidateRequest��NoYes	NoYesId%@ATXApparelAndTextile_en_US:ATXL00050GenerateProdBOM�ATXBOMTypeTable   �    �	BOMTypeId�	
BOMTypeIdx�@ATXAT:NewLabel53!ATXBOMTypeTable$
BOMTypeIdx9  �3	BOMTypeId4Description�� �	 
 8public class ATXProdCutPackagesPost extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��	   �ProdId��ProdCutPackageId��InventSizeId��CutQty��
RouteOprId��WrkCtrId��	TransDate��TurnId��	CreatedBy�	@SYS35893General�   �    	ProdIdProdId��    	ATXProdCutPackageIdProdCutPackageId��    	EcoResSizeNameInventSizeId��    	ATXCutQtyCutQty��    	
RouteOprId
RouteOprId��    	TransDate	TransDate��	WrkCtrIdWrkCtrId��		ATXTurnIdTurnId�   �    �ProdId��ProdCutPackageId�	ProdPackageIdx�@ATXAT:NewLabel296   � 	
find   � 
_packageId ATXProdCutPackageId�� _oprId 
RouteOprId�� false
_forUpdate boolean��  ATXProdCutPackagesPost� �  !ATXProdCutPackagesPost9  �3ProdId4ProdCutPackageId�� �3public class ATXSpreadingTable extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �	Spreading��Description�Overview�   �  	ATXSpreading	Spreading��	DescriptionDescription�ATXSpreadingTable   �    �	Spreading�	SpreadingIdx�   � 	
find   � 
_spreading ATXSpreading�� false
_forUpdate boolean��  ATXSpreadingTable� �!ATXSpreadingTable9  ��� �	SeasonIdx	 
   0public class ATXSeasonTable extends common
{
}Storage for season catalog   �   �SeasonId��Description�
AutoReport��   �SeasonId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SeasonId��Description�	@SYS35893Overview�   �  	ATXSeasonId SeasonId��	DescriptionDescription�ATXSeasonFormDisplay   �    �SeasonId�		SeasonIdx�@ATXAT:NewLabel88   � 	
find   � 	_seasonId ATXSeasonId�� false
_forUpdate boolean��  ATXSeasonTable� �� 	
exist   � 	_seasonId ATXSeasonId��  boolean� �  !ATXSeasonTable$	SeasonIdx9  �3SeasonId4Description�� �"@DMF:StagingDeveloperDocumentation   � 
AutoReport�� 
AutoLookup��  AutoIdentification�� AutoSummary�� 
AutoBrowse��   �DefinitionGroup��
IsSelected��TransferStatus��ExecutionId� @DMF:StagingExtensionGroupExtensionList�   �  	DMFDefinitionGroupName  DefinitionGroup<   ��  	DMFExecutionId  ExecutionIdZ   ��NoYes	DMFIsSelected 
IsSelected��DMFTransferStatus TransferStatus��	BasicCalenderId BasicCalendarId��  	
CalendarId  
CalendarId��	CalendarName Name��StandardWorkDayHours StandardWorkDayHours�WorkCalendarTable   �    �DefinitionGroup��ExecutionId��
CalendarId� 	
StagingIdx�	@SYS11839!ATXWorkCalendarDataStaging$
StagingIdx%   �    �
CalendarId
CalendarId
CalendarId�(@DMF:StagingToDataEntityRelationshipRole 	
DataEntityATXWorkCalendarDataEntity    �&
StagingIdx(  0 3
CalendarId4Name�� �7public class ATXSewStitchesPerInch extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �Description��
StitchType��StitchPerInch��
SewMachine��Notes�Overview�   �	DescriptionDescription��	Description@ATXPLM:NewLabel19
StitchType��	Description@ATXPLM:NewLabel20StitchPerInch��	Description@ATXPLM:NewLabel21
SewMachine��	Description@ATXPLM:NewLabel22Notes��	
RouteOprId
RouteOprId��	ItemIdItemId�@ATXPLM:NewLabel20!ATXSewStitchesPerInch%   �   �
RouteOprId
RouteOprIdOprId��ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �SampleTypeIdxATXPLM	 
   4public class ATXSampleTypeTable extends common
{
}   �   �SampleTypeId��Description�
AutoReport��   �SampleTypeId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SampleTypeId��Description��SamplingPhaseId�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �	ATXSampleTypeIdSampleTypeId��	DescriptionDescription��	ATXSamplingPhaseIdSamplingPhaseId�ATXSampleTypeFormDisplay   �    �SampleTypeId�	SampleTypeIdx�%@ATXApparelAndTextile_en_US:ATXL00027   � 	
find   � _sampleType ATXSampleTypeId�� false
_forUpdate boolean��  ATXSampleTypeTable� �� 	
exist   � _sampleType ATXSampleTypeId��  boolean� �  !ATXSampleTypeTable$SampleTypeIdx%   �   �SamplingPhaseIdSamplingPhaseIdSamplingPhaseId�ATXSamplingPhaseATXSamplingPhase�9  �3SampleTypeId4Description�� �Apublic class ATXRouteSubOperationsAttributes extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �	Attribute��Description��StandardValue��
LowerLimit��
UpperLimit�General�   �RefRecIdATXRouteSubOperations��Customer ContentRefRecId	@SYS77030 	Attribute��Customer ContentRefRecId	@SYS40283Value��	DescriptionDescription��InventTestLowerLimit
LowerLimit��InventTestUpperLimit
UpperLimit��InventTestStandardValueStandardValue�@ATXAT:NewLabel306!ATXRouteSubOperationsAttributes%   �   �ATXRouteSubOperationsATXRouteSubOperationsRecId�ATXRouteSubOperationsATXRouteSubOperations��   �	Attribute	AttributeRecId�EcoResAttributeEcoResAttribute��   �ValueValueRecId�EcoResValueEcoResValue�9  ��� �WarningGroupIdx7public class ATXEventWarningsGroup extends common
{
}   � DeleteAction1 ATXEventWarningMailList �   �   �WarningGroupId��Description�
AutoReport��   �WarningGroupId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �WarningGroupId��Description�	@SYS35893Overview�   �	ATXWarningGroupIdWarningGroupId��	DescriptionDescription�ATXEventWarningGroupForm   �    �WarningGroupId�	WarningGroupIdx�%@ATXApparelAndTextile_en_US:ATXL00046!ATXEventWarningsGroup$WarningGroupIdx9  �3WarningGroupId4Description�� �InventTransIdx;public class ATXBreakdownOrderLine extends common
{


}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ConfigId��InventSizeId��InventColorId��InventStyleId��QtyOrig��Qty��QtyEnd��
SalesPrice�@ATXAT:NewLabel9Request�   �	BOMIdBOMId��	EcoResConfigurationNameConfigId��	EcoResColorNameInventColorId��	EcoResSizeNameInventSizeId��	EcoResStyleNameInventStyleId��	InventTransIdInventTransId��	ItemIdItemId��ATXQtyWithoutDecimals@ATXAT:NewLabel44ProdQty��ATXQtyWithoutDecimals@ATXAT:NewLabel43QtyEnd��ATXQtyWithoutDecimals@ATXAT:NewLabel45QtyOrig��	SalesIdSalesId��
SalesPrice
SalesPrice��ATXQtyWithoutDecimals@ATXAT:NewLabel46SplitQty��RefRecIdRefRecId��    QtyQty�   �    �InventTransId��SalesId��BOMId�	InventTransIdx��    �BOMId�	BOMTableIdx�@ATXAT:NewLabel11   � 	
findBySalesTransBOMId   � _salesId SalesId�� _inventTransId InventTransId�� _bomId BomId�� false
_forUpdate boolean��  ATXBreakdownOrderLine� �� 
validateWrite�  boolean� �� 
modifiedField   � _fieldId fieldId��  � �� 
sumQtyLines�  SalesQty� �� 
validateField   � _fieldIdToCheck FieldId��  boolean� �!ATXBreakdownOrderLine$InventTransIdx%   �   �SalesIdSalesIdSalesId�
SalesTable
SalesTable��   �ItemIdItemIdItemId�InventTableInventTable��   �BOMIdBOMIdBOMId�BOMTableBOMTable��   �InventTransIdInventTransIdInventTransId�	SalesLine	SalesLine��   �SalesIdSalesIdATXInventRefId��InventTransIdInventTransIdATXInventRefTransId�	ProdTable	ProdTable�9  �3SalesId4BOMId�� �4public class ATXProdCutPackages extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ProdId��ProdCutPackageId��InventSizeId��CutQty�	@SYS35893General�   �    	ProdIdProdId��    	ATXProdCutPackageIdProdCutPackageId��    	EcoResSizeNameInventSizeId��    	ATXCutQtyCutQty�   �    �ProdId��ProdCutPackageId�	ProdPackageIdx�@ATXAT:NewLabel292!ATXProdCutPackages9  �3ProdId4ProdCutPackageId�� �ATXPLM2public class ATXPreProdTask extends common
{

}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �PreProdTaskId��Name��
AssignedTo�	@SYS35893General�   �  	ATXPreProdTaskId PreProdTaskId��	NameName��HcmWorkerRecId@ATXPLM:NewLabel5
AssignedTo�   �    �PreProdTaskId�	PreProdTaskIdx�@ATXPLM:NewLabel4   � 	
find   � _preProdTaskId ATXPreProdTaskId�� false
_forUpdate boolean��  ATXPreProdTask� �!ATXPreProdTask%   �   �
AssignedTo
AssignedToRecId�RecId		HcmWorker	HcmWorker�9  �3PreProdTaskId�� �4public class ATXTmpInfoLogError extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �	Exception��counter��Error�Overview�   �counter��	Exception	Exception��	Str1260@ATXAT:NewLabel261Error�!ATXTmpInfoLogError9  ��� �Bpublic class ATXCutTechnicalSheetEmbroidery extends common
{
}
   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��
   �CutAccesoryItem��ItemName��	Placement��ClothGarment��EmbroideryType��Length��Width��Stitches��Service��Notes�Overview�   �	ItemIdItemId��	
RouteOprId
RouteOprId��	DescriptionAccesory��Qty@ATXPLM:NewLabel50Length��	Description@ATXPLM:NewLabel28CutDirection��	Description@ATXPLM:NewLabel29Supply��	Description@ATXPLM:NewLabel22Notes��Qty@ATXPLM:NewLabel32Temp��Qty@ATXPLM:NewLabel52Stitches��Qty@ATXPLM:NewLabel34Pressure��	Description@ATXPLM:NewLabel35PressureUOM��	ItemId@ATXPLM:NewLabel31CutAccesoryItem��	Description@ATXPLM:NewLabel38BendingType��	Description@ATXPLM:NewLabel26	Placement��	Description@ATXPLM:NewLabel21
SewMachine��Qty@ATXPLM:NewLabel51Width��	Description@ATXPLM:NewLabel40ClothGarment��	Description@ATXPLM:NewLabel41SendBy��	Description@ATXPLM:NewLabel42Sleeves��	Description@ATXPLM:NewLabel43SpecialComponent��	Description@ATXPLM:NewLabel44Service��	Description@ATXPLM:NewLabel49EmbroideryType��	Description@ATXPLM:NewLabel47Combinations�   � 
ItemName�  ItemName� �!ATXCutTechnicalSheetEmbroidery%   �   �ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �7public class ATXBOMBlockingTable extends common
{
}
   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	ItemIdItemId��	BOMIdBOMId�@ATXAT:NewLabel72!ATXBOMBlockingTable9  �3ItemId4BOMId�� �ItemDivisionIdx	 
   6public class ATXItemDivisionTable extends common
{
}!Storage for item division catalog   �   �ItemDivisionId��Description�
AutoReport��   �ItemDivisionId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ItemDivisionId��Description�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �  	ATXItemDivisionId ItemDivisionId��	DescriptionDescription�ATXItemDivisionFormDisplay   �    �ItemDivisionId�	ItemDivisionIdx�@ATXAT:NewLabel86   � 	
find   � _itemDivisionId ATXItemDivisionId�� false
_forUpdate boolean��  ATXItemDivisionTable� �� 	
exist   � _itemDivisionId ATXItemDivisionId��  boolean� �  !ATXItemDivisionTable$ItemDivisionIdx%   �   �ItemDivisionIdItemDivisionIdItemDivisionId�ATXItemDivisionTableATXItemDivisionTable�9  �3ItemDivisionId4Description�� �.public class ATXTurnTable extends common
{
}   �
AutoReport��   �TurnId��FromTime��ToTime��
CalendarId�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �TurnId��FromTime��ToTime��Split��
CalendarId�Overview��   �TurnId��Name�SimpleGroup�   �	
CalendarId
CalendarId��FromTimeFromTime��	NameName��NoYes	NoYesIdSplit��ToTimeToTime��		ATXTurnIdTurnId�   �    �TurnId�	TurnIdx�   � 
getCalendar   � 	_wrkctrId WrkCtrId��  
CalendarId��� 	
exist   � _turnId 	ATXTurnId��  boolean� �� 	
	existTurn   � _turnId 	ATXTurnId��  boolean� �� 	
find   � _turnId 	ATXTurnId�� false_update boolean��  ATXTurnTable� �� 	
findBySystemTime   � 	_wrkctrId WrkCtrId�� 	timeNow()_time FromTime��  ATXTurnTable� �� 	
getCalendarFromWRKCTR   � 	_wrkctrId WrkCtrId��  
CalendarId� �� 	
hours   � _turnId 	ATXTurnId�� 	_wrkctrId Wrkctrid��  Hours� �!ATXTurnTable%   �   �
CalendarId
CalendarId
CalendarId�WorkCalendarTableWorkCalendarTable�9  ��� �ReqIdx5public class ATXRequestOrderLine extends common
{
}   �   �InventTransOriginId��RequestOrderId��RequestOrderUpdateId��ItemId��InventDimId��QtyOrig��LineAmountOrig��
RequestQty��
SalesPrice��
LineAmount��SeasonId��RequestOrderDate��RequestOrderCancelDate��ReviewedOrderDate��BranchId��ItemDivisionId��LineDisc��LinePercent�
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��
   �ItemId��LineNum��QtyOrig��
RequestQty��
SalesPrice��LineAmountOrig��
LineAmount��RequestOrderDate��RequestOrderCancelDate��ReviewedOrderDate�	@SYS35893Overview�   �		DlvModeId	DlvModeId��	InventDimIdInventDimId��	TradeInventTransIdInventTransIdOrigin��	ATXItemDivisionIdItemDivisionId��	ItemIdItemId��SalesLineAmount
LineAmount��Amount@ATXAT:NewLabel89LineAmountOrig��SalesQty@ATXAT:NewLabel45QtyOrig��ATXRequestOrderCancelDateRequestOrderCancelDate��ATXRequestOrderDateRequestOrderDate��	ATXRequestOrderIdRequestOrderId��ATXRequestOrderUpdateIdRequestOrderUpdateId��SalesQty@ATXAT:NewLabel49
RequestQty��ATXReviewedOrderDateReviewedOrderDate��
SalesPrice
SalesPrice��	ATXSeasonIdSeasonId��	ATXBranchIdBranchId��SalesLineDiscLineDisc��SalesLinePercentLinePercent��InventTransOriginIdInventTransOriginId��	ATXDestinationPlaceIdDestinationPlaceId��LineNumLineNum�   �    �RequestOrderId�	ReqIdx�@ATXAT:NewLabel83   � 
insert�  � ��     !SysClientCacheDataMethodAttribute     True��
displayConfigName�  
ConfigName� �� 
	inventDim�  	InventDim� �� 
inventTable�  InventTable� �� 
modifiedField   � _fieldId FieldId��  � �� 
calcLineAmount�  � �� 
requestOrderHeader�  ATXRequestOrderHeader� �� 
setInventDimId   � _inventDimId InventDimId�� InventDim::find(_inventDimId)
_inventDim 	InventDim��  � �� 
update�  � �� 
updateRequestOrderCancelDate�  � �� 
updateRequestOrderDate�  � �� 
updateReviewedOrderDate�  � �� 
updateSalesPrice�  � �� 
updateShipmentOrderDate�  � �� 
validateDelete�  boolean� �� 	
findByRecId   � _recId RecId�� false
_forUpdate boolean��  ATXRequestOrderLine� �� 
RequestSizeId�  EcoResSizeName� ��     !SysClientCacheDataMethodAttribute     True��
displayItemName�  ItemName� �� 
validateWrite�  boolean� �� 
aosValidateInsert�  boolean� �� 
	initValue�  � �� 	
getLastLineNum   � _requestOrderId ATXRequestOrderId�� _requestOrderUpdateId ATXRequestOrderUpdateId��  LineNum� �!ATXRequestOrderLine%   �   �RequestOrderIdRequestOrderIdRequestOrderId��RequestOrderUpdateIdRequestOrderUpdateIdRequestOrderUpdateId�ATXRequestOrderUpdatesATXRequestOrderUpdates��   �ItemDivisionIdItemDivisionIdItemDivisionId�ATXItemDivisionTableATXItemDivisionTable��   �DestinationPlaceIdDestinationPlaceIdDestinationPlaceId�ATXDestinationPlaceATXDestinationPlace��   �SeasonIdSeasonIdSeasonId�ATXSeasonTableATXSeasonTable�9  �3RequestOrderId4ItemId�� �8public class ATXProductOvercutSetup extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��	   �ProductOvercutId��FromQty��ToQty��PercentAmount��RoundOffType��BOMRoundUpQty��configId��InventColorId��Qty�	@SYS35893Overview�	   �BOMRoundUpQtyBOMRoundUpQty��	EcoResItemConfigurationNameconfigId��FromQtyFromQty��	EcoResItemColorNameInventColorId��PercentAmountPercentAmount��  	ATXProductOvercutId ProductOvercutId��FromQty@ATXAT:NewLabel274Qty��RoundOffTypeRoundOffType��AmountQuantityToToQty�@ATXAT:NewLabel133   � 
displayDescription�  Description� �� 	
find   � _productOvercutId_AT ATXProductOvercutId�� _qty Qty�� 	_configId EcoResConfigurationName�� _inventColorId EcoResColorName��  ATXProductOvercutSetup� �!ATXProductOvercutSetup%   �   �ProductOvercutIdProductOvercutIdProductOvercutId�ATXProductOvercutATXProductOvercut�9  ��� �9public class ATXEventWarningMailList extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �WarningGroupId��MailList�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �	ATXWarningGroupIdWarningGroupId��	Notes%@ATXApparelAndTextile_en_US:ATXL00047MailList�@ATXAT:NewLabel78!ATXEventWarningMailList%   �   �WarningGroupIdWarningGroupIdWarningGroupId�ATXEventWarningGroupATXEventWarningsGroup�9  ��� �ProductOvercutIdx3public class ATXProductOvercut extends common
{
}   �
AutoReport��   �ProductOvercutId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ProductOvercutId��Description�	@SYS35893Overview�   �	DescriptionDescription��  	ATXProductOvercutIdProductOvercutId�ATXProductOvercut   �    �ProductOvercutId�	ProductOvercutIdx�@ATXAT:NewLabel70   � 
modifiedField   � _fieldId FieldId��  � �� 	
find   � _productOvercutId ATXProductOvercutId�� false
_forUpdate boolean��  ATXProductOvercut� �!ATXProductOvercut$ProductOvercutIdx9  �3ProductOvercutId4Description�� �5public class ATXProdQualityTable extends common
{
}   �
AutoReport��   �ProdQualityId��Description�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ProdQualityId��Description�Overview�   �	ATXProdQualityIdProdQualityId��	DescriptionDescription�ATXProdQualityTable   �    �ProdQualityId�	ProdQualityIdx�   � 
checkFixReference�  � �� 
insert�  � �� 	
exist   � _quality ATXProdQualityId��  boolean� �� 	
find   � _quality ATXProdQualityId�� falseupdate boolean��  ATXProdQualityTable� �!ATXProdQualityTable$ProdQualityIdx9  ��� �Cpublic class ATXSewOperationMeasurements extends common
{
    
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �SubOperationId��SubOperationName��ToleranceUp��ToleranceDown��	SizeCopy1��	SizeCopy2��	SizeCopy3��	SizeCopy4��	SizeCopy5��	SizeCopy6��	SizeCopy7��	SizeCopy8��	SizeCopy9��
SizeCopy10��
SizeCopy11��
SizeCopy12��
SizeCopy13��
SizeCopy14��
SizeCopy15�Overview�   �	ItemIdItemId��	ATXSubOperationIdSubOperationId��	Description@ATXPLM:NewLabel55ToleranceUp��	Description@ATXPLM:NewLabel56ToleranceDown��	DescriptionSize��	DescriptionTalla 1	SizeCopy1��	DescriptionTalla 2	SizeCopy2��	DescriptionTalla 3	SizeCopy3��	DescriptionTalla 4	SizeCopy4��	DescriptionTalla 5	SizeCopy5��	DescriptionTalla 6	SizeCopy6��	DescriptionTalla 7	SizeCopy7��	DescriptionTalla 8	SizeCopy8��	DescriptionTalla 9	SizeCopy9��	DescriptionTalla 10
SizeCopy10��	DescriptionTalla 11
SizeCopy11��	DescriptionTalla 12
SizeCopy12��	DescriptionTalla 13
SizeCopy13��	DescriptionTalla 14
SizeCopy14��	DescriptionTalla 15
SizeCopy15�   � 
SubOperationName�  Name� �!ATXSewOperationMeasurements%   �   �ItemIdItemIdItemRelation�RouteOprRouteOpr��   �SubOperationIdSubOperationIdSubOperationId�	ATXSubOperationATXSubOperation�9  ��� �CustClassIdx3public class ATXCustClassTable extends common
{
}   �
AutoReport��   �CustClassId��DeptName��Dept��Name�
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �CustClassId��DeptName��Dept��Name�%@ATXApparelAndTextile_en_US:ATXL00009Overview�   �	NameName��	NameDeptName��	NameDept��	ATXCustClassIdCustClassId�   �    �CustClassId�	CustClassIdx�@ATXAT:NewLabel82   � 
displayData�  Description255� �� 	
find   � _custClassId ATXCustClassId�� false
_forUpdate boolean��  ATXCustClassTable� �!ATXCustClassTable$CustClassIdx9  ��� �7public class ATXRouteSubOperations extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse��   �ItemId��
RouteOprId��SubOperationId��displaySubOperationName��SequenceNumber�@ATXAT:NewLabel214General�   �  	ATXSubOperationId SubOperationId��    	
RouteOprId 
RouteOprId��	ItemIdItemId��SequenceNumberSequenceNumber�   �   �ItemId��
RouteOprId��SubOperationId�	SubOperationId�   �     SysClientCacheDataMethod     True��
displaySubOperationName�  Name� �!ATXRouteSubOperations%   �   �SubOperationIdSubOperationIdSubOperationId�ATXSubOperationATXSubOperation��   �
RouteOprId
RouteOprIdOprId�	ProdRoute	ProdRoute��   �
RouteOprId
RouteOprIdOprId��ItemIdItemIdItemRelation�RouteOprRouteOpr�9  ��� �6public class ATXRouteCardRouteTmp extends common
{
}   �
AutoReport��
AutoLookup�� AutoIdentification��AutoSummary��
AutoBrowse�   �	
RouteOprIdOprId��	NameName��	DescriptionOprIdBarCode��OprNumOprNum�!ATXRouteCardRouteTmp9  �1 �