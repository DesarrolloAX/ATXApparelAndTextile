   ATXBOM�tg5    �  ATXBOMMacro�tg5�  �  ATXBOMTableExistsJoinTemplate�tg5�  �   ATXScannerStationLogCatch�tg5O  �   � � ATXBOM�#define.Template                ('PLANTILLA')
#define.SalesOrder              ('S.O.')
#define.ProductionOrder         ('P.O.')
#define.ExclamationMark         ('!')
#define.InventColor             ('InventColor')
#define.InventSize              ('InventSize')
#define.InventColorId           ('InventColorId')
#define.InventSizeId            ('InventSizeId')
#define.ConfigId                ('ConfigTable')
#define.Empy                    ('')
#define.DummyValue              ('#')
#define.ItemFieldName           ('ItemId')
#define.NameFieldName           ('Name')
#define.CharBOMSeparator        ('-')
#define.CharItemDimSeparator    (' ')
#define.FirstQualityBOM         ('PRIMERA')
#define.USD('USD')
#define.MXN('MXN')�� � ATXBOMMacro�#define.Template                ('PLANTILLA')
#define.SalesOrder              ('S.O.')
#define.ProductionOrder         ('P.O.')
#define.ExclamationMark         ('!')
#define.InventColor             ('InventColor')
#define.InventSize              ('InventSize')
#define.InventColorId           ('InventColorId')
#define.InventSizeId            ('InventSizeId')
#define.ConfigId                ('ConfigTable')
#define.Empy                    ('')
#define.DummyValue              ('#')
#define.ItemFieldName           ('ItemId')
#define.NameFieldName           ('Name')
#define.CharBOMSeparator        ('-')
#define.CharItemDimSeparator    (' ')�� � ATXBOMTableExistsJoinTemplate�/* %1 bomTable           */
/* %2 %2     */

exists join %1
where %1.BOMId == %2.BOMId
&& %1.ATXBOMType == ATXBOMType::Template
;
/* */�� � ATXScannerStationLogCatch�//> Form log grid
catch (Exception::UpdateConflictNotRecovered)
{
    error("Conflicto de actualización. Operación cancelada.");
    this.updateInfoLogView();
}
catch
{
    this.updateInfoLogView();
}�