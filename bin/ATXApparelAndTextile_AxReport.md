   ATXRouteCard�tg5    � � :   Q     T ATXRouteCardHeaderTmp.1.CustName	@SYS80991Auto
CustName �T)ATXRouteCardHeaderTmp.1.CustPurchaseOrder	@SYS23422Auto
CustPurchaseOrder �T$ATXRouteCardHeaderTmp.1.DeliveryDate@SYS7402System.DateTimeAuto
DeliveryDate �T*ATXRouteCardHeaderTmp.1.DestinationPlaceId@ATXAT:NewLabel87Auto
DestinationPlaceId �T%ATXRouteCardHeaderTmp.1.InventBatchId	@SYS53635Auto
InventBatchId �TATXRouteCardHeaderTmp.1.ItemId	@SYS12836Auto
ItemId �T ATXRouteCardHeaderTmp.1.ItemName@SYS5398Auto
ItemName �TATXRouteCardHeaderTmp.1.ProdId@SYS4398Auto
ProdId �T%ATXRouteCardHeaderTmp.1.ProdIdBarcode@SYS7576Auto
ProdIdBarcode �TATXRouteCardHeaderTmp.1.SalesId@SYS9694Auto
SalesId �T ATXRouteCardHeaderTmp.1.SeasonId@ATXAT:NewLabel77Auto
SeasonId �Header   WAX_PartitionKeySystem.StringAX_PartitionKeyAX_PartitionKey�WAX_CompanyNameSystem.StringAX_CompanyNameAX_CompanyName�WAX_UserContextSystem.StringAX_UserContextAX_UserContext�WAX_RenderingCultureSystem.StringAX_RenderingCultureAX_RenderingCulture�WAX_ReportContextSystem.StringAX_ReportContextAX_ReportContext�WAX_RdpPreProcessedIdSystem.StringAX_RdpPreProcessedIdAX_RdpPreProcessedId�WRecIdSystem.Int64RecIdHeader_RecId�W
RouteOprIdSystem.String
RouteOprIdHeader_RouteOprId�	2SELECT * FROM ATXRouteCardDP.ATXRouteCardHeaderTmp�Q     T'ATXRouteCardBreakdownTmp.1.InventSizeId	@SYS73727Auto
InventSizeId �TATXRouteCardBreakdownTmp.1.Qty	@SYS14578System.DoubleAuto
Qty �	Breakdown   WAX_PartitionKeySystem.StringAX_PartitionKeyAX_PartitionKey�WAX_CompanyNameSystem.StringAX_CompanyNameAX_CompanyName�WAX_UserContextSystem.StringAX_UserContextAX_UserContext�WAX_RenderingCultureSystem.StringAX_RenderingCultureAX_RenderingCulture�WAX_ReportContextSystem.StringAX_ReportContextAX_ReportContext�WAX_RdpPreProcessedIdSystem.StringAX_RdpPreProcessedIdAX_RdpPreProcessedId�WRecIdSystem.Int64RecIdHeader_RecId�W
RouteOprIdSystem.String
RouteOprIdHeader_RouteOprId�	5SELECT * FROM ATXRouteCardDP.ATXRouteCardBreakdownTmp�Q     TATXRouteCardRouteTmp.1.Name@SYS7399Auto
Name �TATXRouteCardRouteTmp.1.OprId
@SYS101237Auto
OprId �T#ATXRouteCardRouteTmp.1.OprIdBarCode@SYS7576Auto
OprIdBarCode �TATXRouteCardRouteTmp.1.OprNum@SYS5793System.Int32Auto
OprNum �Route   WAX_PartitionKeySystem.StringAX_PartitionKeyAX_PartitionKey�WAX_CompanyNameSystem.StringAX_CompanyNameAX_CompanyName�WAX_UserContextSystem.StringAX_UserContextAX_UserContext�WAX_RenderingCultureSystem.StringAX_RenderingCultureAX_RenderingCulture�WAX_ReportContextSystem.StringAX_ReportContextAX_ReportContext�WAX_RdpPreProcessedIdSystem.StringAX_RdpPreProcessedIdAX_RdpPreProcessedId�WRecIdSystem.Int64RecIdHeader_RecId�W
RouteOprIdSystem.String
RouteOprIdHeader_RouteOprId�	1SELECT * FROM ATXRouteCardDP.ATXRouteCardRouteTmp��
Parameters   }ReportParameterDefault�AX_PartitionKey
 �ReportParameterValue��}ReportParameterDefault�AX_CompanyName
 �ReportParameterValue��}ReportParameterDefault�AX_UserContext
 �ReportParameterValue��}ReportParameterDefault�AX_RenderingCulture
 �ReportParameterValue��}ReportParameterDefault�AX_ReportContext
 �ReportParameterValue��}ReportParameterDefault�AX_RdpPreProcessedId
 �ReportParameterValue��}System.Int64ReportParameterDefault�Header_RecId
 �ReportParameterValue��}ReportParameterDefault�Header_RouteOprId�ReportParameterValue���   �Y%ReportDisableIndividualTransformation�Design��<?xml version="1.0" encoding="utf-8"?>
<Report xmlns:rd="http://schemas.microsoft.com/SQLServer/reporting/reportdesigner" xmlns:cl="http://schemas.microsoft.com/sqlserver/reporting/2010/01/componentdefinition" xmlns="http://schemas.microsoft.com/sqlserver/reporting/2010/01/reportdefinition">
  <AutoRefresh>0</AutoRefresh>
  <DataSources>
    <DataSource Name="AutoGen__ReportDataProvider">
      <Transaction>true</Transaction>
      <ConnectionProperties>
        <DataProvider>AXREPORTDATAPROVIDER</DataProvider>
        <ConnectString />
        <IntegratedSecurity>true</IntegratedSecurity>
      </ConnectionProperties>
      <rd:DataSourceID>bc71c740-dc49-4d51-831a-71ed83af428e</rd:DataSourceID>
    </DataSource>
  </DataSources>
  <DataSets>
    <DataSet Name="Header">
      <Query>
        <DataSourceName>AutoGen__ReportDataProvider</DataSourceName>
        <QueryParameters>
          <QueryParameter Name="AX_PartitionKey">
            <Value>=Parameters!AX_PartitionKey.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_CompanyName">
            <Value>=Parameters!AX_CompanyName.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_UserContext">
            <Value>=Parameters!AX_UserContext.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_RenderingCulture">
            <Value>=Parameters!AX_RenderingCulture.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_ReportContext">
            <Value>=Parameters!AX_ReportContext.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_RdpPreProcessedId">
            <Value>=Parameters!AX_RdpPreProcessedId.Value</Value>
          </QueryParameter>
          <QueryParameter Name="RecId">
            <Value>=Parameters!Header_RecId.Value</Value>
          </QueryParameter>
          <QueryParameter Name="RouteOprId">
            <Value>=Parameters!Header_RouteOprId.Value</Value>
          </QueryParameter>
        </QueryParameters>
        <CommandText>SELECT * FROM ATXRouteCardDP.ATXRouteCardHeaderTmp</CommandText>
        <rd:UseGenericDesigner>true</rd:UseGenericDesigner>
      </Query>
      <Fields>
        <Field Name="CustName">
          <DataField>ATXRouteCardHeaderTmp.1.CustName</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="CustPurchaseOrder">
          <DataField>ATXRouteCardHeaderTmp.1.CustPurchaseOrder</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="DeliveryDate">
          <DataField>ATXRouteCardHeaderTmp.1.DeliveryDate</DataField>
          <rd:TypeName>System.DateTime</rd:TypeName>
        </Field>
        <Field Name="DestinationPlaceId">
          <DataField>ATXRouteCardHeaderTmp.1.DestinationPlaceId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="InventBatchId">
          <DataField>ATXRouteCardHeaderTmp.1.InventBatchId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="ItemId">
          <DataField>ATXRouteCardHeaderTmp.1.ItemId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="ItemName">
          <DataField>ATXRouteCardHeaderTmp.1.ItemName</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="ProdId">
          <DataField>ATXRouteCardHeaderTmp.1.ProdId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="ProdIdBarcode">
          <DataField>ATXRouteCardHeaderTmp.1.ProdIdBarcode</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="SalesId">
          <DataField>ATXRouteCardHeaderTmp.1.SalesId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="SeasonId">
          <DataField>ATXRouteCardHeaderTmp.1.SeasonId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
      </Fields>
      <rd:DataSetInfo>
        <rd:DataSetName>Header</rd:DataSetName>
        <rd:TableName>Fields</rd:TableName>
        <rd:TableAdapterFillMethod>Fill</rd:TableAdapterFillMethod>
        <rd:TableAdapterGetDataMethod>GetData</rd:TableAdapterGetDataMethod>
        <rd:TableAdapterName>FieldsTableAdapter</rd:TableAdapterName>
      </rd:DataSetInfo>
    </DataSet>
    <DataSet Name="Breakdown">
      <Query>
        <DataSourceName>AutoGen__ReportDataProvider</DataSourceName>
        <QueryParameters>
          <QueryParameter Name="AX_PartitionKey">
            <Value>=Parameters!AX_PartitionKey.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_CompanyName">
            <Value>=Parameters!AX_CompanyName.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_UserContext">
            <Value>=Parameters!AX_UserContext.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_RenderingCulture">
            <Value>=Parameters!AX_RenderingCulture.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_ReportContext">
            <Value>=Parameters!AX_ReportContext.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_RdpPreProcessedId">
            <Value>=Parameters!AX_RdpPreProcessedId.Value</Value>
          </QueryParameter>
          <QueryParameter Name="RecId">
            <Value>=Parameters!Header_RecId.Value</Value>
          </QueryParameter>
          <QueryParameter Name="RouteOprId">
            <Value>=Parameters!Header_RouteOprId.Value</Value>
          </QueryParameter>
        </QueryParameters>
        <CommandText>SELECT * FROM ATXRouteCardDP.ATXRouteCardBreakdownTmp</CommandText>
        <rd:UseGenericDesigner>true</rd:UseGenericDesigner>
      </Query>
      <Fields>
        <Field Name="InventSizeId">
          <DataField>ATXRouteCardBreakdownTmp.1.InventSizeId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="Qty">
          <DataField>ATXRouteCardBreakdownTmp.1.Qty</DataField>
          <rd:TypeName>System.Double</rd:TypeName>
        </Field>
      </Fields>
      <rd:DataSetInfo>
        <rd:DataSetName>Breakdown</rd:DataSetName>
        <rd:TableName>Fields</rd:TableName>
        <rd:TableAdapterFillMethod>Fill</rd:TableAdapterFillMethod>
        <rd:TableAdapterGetDataMethod>GetData</rd:TableAdapterGetDataMethod>
        <rd:TableAdapterName>FieldsTableAdapter</rd:TableAdapterName>
      </rd:DataSetInfo>
    </DataSet>
    <DataSet Name="Route">
      <Query>
        <DataSourceName>AutoGen__ReportDataProvider</DataSourceName>
        <QueryParameters>
          <QueryParameter Name="AX_PartitionKey">
            <Value>=Parameters!AX_PartitionKey.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_CompanyName">
            <Value>=Parameters!AX_CompanyName.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_UserContext">
            <Value>=Parameters!AX_UserContext.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_RenderingCulture">
            <Value>=Parameters!AX_RenderingCulture.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_ReportContext">
            <Value>=Parameters!AX_ReportContext.Value</Value>
          </QueryParameter>
          <QueryParameter Name="AX_RdpPreProcessedId">
            <Value>=Parameters!AX_RdpPreProcessedId.Value</Value>
          </QueryParameter>
          <QueryParameter Name="RecId">
            <Value>=Parameters!Header_RecId.Value</Value>
          </QueryParameter>
          <QueryParameter Name="RouteOprId">
            <Value>=Parameters!Header_RouteOprId.Value</Value>
          </QueryParameter>
        </QueryParameters>
        <CommandText>SELECT * FROM ATXRouteCardDP.ATXRouteCardRouteTmp</CommandText>
        <rd:UseGenericDesigner>true</rd:UseGenericDesigner>
      </Query>
      <Fields>
        <Field Name="Name">
          <DataField>ATXRouteCardRouteTmp.1.Name</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="OprId">
          <DataField>ATXRouteCardRouteTmp.1.OprId</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="OprIdBarCode">
          <DataField>ATXRouteCardRouteTmp.1.OprIdBarCode</DataField>
          <rd:TypeName>System.String</rd:TypeName>
        </Field>
        <Field Name="OprNum">
          <DataField>ATXRouteCardRouteTmp.1.OprNum</DataField>
          <rd:TypeName>System.Int32</rd:TypeName>
        </Field>
      </Fields>
      <rd:DataSetInfo>
        <rd:DataSetName>Route</rd:DataSetName>
        <rd:TableName>Fields</rd:TableName>
        <rd:TableAdapterFillMethod>Fill</rd:TableAdapterFillMethod>
        <rd:TableAdapterGetDataMethod>GetData</rd:TableAdapterGetDataMethod>
        <rd:TableAdapterName>FieldsTableAdapter</rd:TableAdapterName>
      </rd:DataSetInfo>
    </DataSet>
  </DataSets>
  <ReportSections>
    <ReportSection>
      <Body>
        <ReportItems>
          <Tablix Name="Tablix1">
            <TablixCorner>
              <TablixCornerRows>
                <TablixCornerRow>
                  <TablixCornerCell>
                    <CellContents>
                      <Textbox Name="Textbox28">
                        <CanGrow>true</CanGrow>
                        <KeepTogether>true</KeepTogether>
                        <Paragraphs>
                          <Paragraph>
                            <TextRuns>
                              <TextRun>
                                <Value>=Labels!@ATXAT:NewLabel227</Value>
                                <Style>
                                  <FontSize>8pt</FontSize>
                                </Style>
                              </TextRun>
                            </TextRuns>
                            <Style />
                          </Paragraph>
                        </Paragraphs>
                        <rd:DefaultName>Textbox28</rd:DefaultName>
                        <Style>
                          <Border>
                            <Color>LightGrey</Color>
                            <Style>Solid</Style>
                          </Border>
                          <PaddingLeft>2pt</PaddingLeft>
                          <PaddingRight>2pt</PaddingRight>
                          <PaddingTop>2pt</PaddingTop>
                          <PaddingBottom>2pt</PaddingBottom>
                        </Style>
                      </Textbox>
                    </CellContents>
                  </TablixCornerCell>
                </TablixCornerRow>
              </TablixCornerRows>
            </TablixCorner>
            <TablixBody>
              <TablixColumns>
                <TablixColumn>
                  <Width>0.66667in</Width>
                </TablixColumn>
                <TablixColumn>
                  <Width>0.55208in</Width>
                </TablixColumn>
              </TablixColumns>
              <TablixRows>
                <TablixRow>
                  <Height>0.25in</Height>
                  <TablixCells>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="Qty">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Sum(Fields!Qty.Value)</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                    <Format>#,0.00;-#,0.00;'0.00'</Format>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>Qty</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="Qty1">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Sum(Fields!Qty.Value)</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                    <Format>#,0.00;-#,0.00;'0.00'</Format>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>Qty1</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                  </TablixCells>
                </TablixRow>
              </TablixRows>
            </TablixBody>
            <TablixColumnHierarchy>
              <TablixMembers>
                <TablixMember>
                  <Group Name="ColumnGroup">
                    <GroupExpressions>
                      <GroupExpression>=Fields!InventSizeId.Value</GroupExpression>
                    </GroupExpressions>
                  </Group>
                  <TablixHeader>
                    <Size>0.25in</Size>
                    <CellContents>
                      <Textbox Name="InventSizeId">
                        <CanGrow>true</CanGrow>
                        <KeepTogether>true</KeepTogether>
                        <Paragraphs>
                          <Paragraph>
                            <TextRuns>
                              <TextRun>
                                <Value>=Fields!InventSizeId.Value</Value>
                                <Style>
                                  <FontSize>8pt</FontSize>
                                </Style>
                              </TextRun>
                            </TextRuns>
                            <Style />
                          </Paragraph>
                        </Paragraphs>
                        <rd:DefaultName>InventSizeId</rd:DefaultName>
                        <CustomProperties>
                          <CustomProperty>
                            <Name>AXDataType</Name>
                            <Value>String</Value>
                          </CustomProperty>
                          <CustomProperty>
                            <Name>AXEDTFormat</Name>
                            <Value>ATXRouteCardBreakdownTmp.InventSizeId</Value>
                          </CustomProperty>
                          <CustomProperty>
                            <Name>AXEDTTextAlign</Name>
                            <Value>ATXRouteCardBreakdownTmp.InventSizeId</Value>
                          </CustomProperty>
                          <CustomProperty>
                            <Name>AXEDTDirection</Name>
                            <Value>ATXRouteCardBreakdownTmp.InventSizeId</Value>
                          </CustomProperty>
                        </CustomProperties>
                        <Style>
                          <Border>
                            <Color>LightGrey</Color>
                            <Style>Solid</Style>
                          </Border>
                          <PaddingLeft>2pt</PaddingLeft>
                          <PaddingRight>2pt</PaddingRight>
                          <PaddingTop>2pt</PaddingTop>
                          <PaddingBottom>2pt</PaddingBottom>
                        </Style>
                      </Textbox>
                    </CellContents>
                  </TablixHeader>
                </TablixMember>
                <TablixMember>
                  <TablixHeader>
                    <Size>0.25in</Size>
                    <CellContents>
                      <Textbox Name="Textbox24">
                        <CanGrow>true</CanGrow>
                        <KeepTogether>true</KeepTogether>
                        <Paragraphs>
                          <Paragraph>
                            <TextRuns>
                              <TextRun>
                                <Value EvaluationMode="Constant">Total</Value>
                                <Style>
                                  <FontSize>8pt</FontSize>
                                </Style>
                              </TextRun>
                            </TextRuns>
                            <Style />
                          </Paragraph>
                        </Paragraphs>
                        <rd:DefaultName>Textbox24</rd:DefaultName>
                        <Style>
                          <Border>
                            <Color>LightGrey</Color>
                            <Style>Solid</Style>
                          </Border>
                          <PaddingLeft>2pt</PaddingLeft>
                          <PaddingRight>2pt</PaddingRight>
                          <PaddingTop>2pt</PaddingTop>
                          <PaddingBottom>2pt</PaddingBottom>
                        </Style>
                      </Textbox>
                    </CellContents>
                  </TablixHeader>
                </TablixMember>
              </TablixMembers>
            </TablixColumnHierarchy>
            <TablixRowHierarchy>
              <TablixMembers>
                <TablixMember>
                  <Group Name="RowGroup">
                    <GroupExpressions>
                      <GroupExpression />
                    </GroupExpressions>
                  </Group>
                  <TablixHeader>
                    <Size>0.47917in</Size>
                    <CellContents>
                      <Textbox Name="Textbox25">
                        <CanGrow>true</CanGrow>
                        <KeepTogether>true</KeepTogether>
                        <Paragraphs>
                          <Paragraph>
                            <TextRuns>
                              <TextRun>
                                <Value>=Labels!@ATXAT:NewLabel228</Value>
                                <Style>
                                  <FontSize>8pt</FontSize>
                                </Style>
                              </TextRun>
                            </TextRuns>
                            <Style />
                          </Paragraph>
                        </Paragraphs>
                        <rd:DefaultName>Textbox25</rd:DefaultName>
                        <Style>
                          <Border>
                            <Color>LightGrey</Color>
                            <Style>Solid</Style>
                          </Border>
                          <PaddingLeft>2pt</PaddingLeft>
                          <PaddingRight>2pt</PaddingRight>
                          <PaddingTop>2pt</PaddingTop>
                          <PaddingBottom>2pt</PaddingBottom>
                        </Style>
                      </Textbox>
                    </CellContents>
                  </TablixHeader>
                </TablixMember>
              </TablixMembers>
            </TablixRowHierarchy>
            <DataSetName>Breakdown</DataSetName>
            <Top>0.13542in</Top>
            <Left>0.2175in</Left>
            <Height>0.5in</Height>
            <Width>1.69792in</Width>
            <Style>
              <Border>
                <Style>None</Style>
              </Border>
            </Style>
          </Tablix>
          <Tablix Name="Tablix2">
            <TablixBody>
              <TablixColumns>
                <TablixColumn>
                  <Width>1in</Width>
                </TablixColumn>
                <TablixColumn>
                  <Width>1in</Width>
                </TablixColumn>
                <TablixColumn>
                  <Width>3.52083in</Width>
                </TablixColumn>
                <TablixColumn>
                  <Width>1.94445in</Width>
                </TablixColumn>
              </TablixColumns>
              <TablixRows>
                <TablixRow>
                  <Height>0.25in</Height>
                  <TablixCells>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="Textbox29">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Labels!@ATXAT:NewLabel229</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                    <FontWeight>Bold</FontWeight>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>Textbox29</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="Textbox31">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Labels!@ATXAT:NewLabel230</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                    <FontWeight>Bold</FontWeight>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>Textbox31</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="Textbox33">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Labels!@ATXAT:NewLabel222</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                    <FontWeight>Bold</FontWeight>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>Textbox33</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="Textbox27">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value />
                                  <Style />
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>Textbox27</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                  </TablixCells>
                </TablixRow>
                <TablixRow>
                  <Height>0.25in</Height>
                  <TablixCells>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="OprNum">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Fields!OprNum.Value</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>OprNum</rd:DefaultName>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="OprId">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Fields!OprId.Value</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>OprId</rd:DefaultName>
                          <CustomProperties>
                            <CustomProperty>
                              <Name>AXDataType</Name>
                              <Value>String</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTFormat</Name>
                              <Value>ATXRouteCardRouteTmp.OprId</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTTextAlign</Name>
                              <Value>ATXRouteCardRouteTmp.OprId</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTDirection</Name>
                              <Value>ATXRouteCardRouteTmp.OprId</Value>
                            </CustomProperty>
                          </CustomProperties>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="OprId1">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Fields!OprId.Value</Value>
                                  <Style>
                                    <FontSize>8pt</FontSize>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style />
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>OprId1</rd:DefaultName>
                          <CustomProperties>
                            <CustomProperty>
                              <Name>AXDataType</Name>
                              <Value>String</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTFormat</Name>
                              <Value>ATXRouteCardRouteTmp.OprId</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTTextAlign</Name>
                              <Value>ATXRouteCardRouteTmp.OprId</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTDirection</Name>
                              <Value>ATXRouteCardRouteTmp.OprId</Value>
                            </CustomProperty>
                          </CustomProperties>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                    <TablixCell>
                      <CellContents>
                        <Textbox Name="OprIdBarCode">
                          <CanGrow>true</CanGrow>
                          <KeepTogether>true</KeepTogether>
                          <Paragraphs>
                            <Paragraph>
                              <TextRuns>
                                <TextRun>
                                  <Value>=Fields!OprIdBarCode.Value</Value>
                                  <Style>
                                    <FontFamily>BC CBar 3 to 1 Narrow</FontFamily>
                                    <FontSize>16pt</FontSize>
                                  </Style>
                                </TextRun>
                              </TextRuns>
                              <Style>
                                <TextAlign>Center</TextAlign>
                              </Style>
                            </Paragraph>
                          </Paragraphs>
                          <rd:DefaultName>OprIdBarCode</rd:DefaultName>
                          <CustomProperties>
                            <CustomProperty>
                              <Name>AXDataType</Name>
                              <Value>String</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTFormat</Name>
                              <Value>ATXRouteCardRouteTmp.OprIdBarCode</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTTextAlign</Name>
                              <Value>ATXRouteCardRouteTmp.OprIdBarCode</Value>
                            </CustomProperty>
                            <CustomProperty>
                              <Name>AXEDTDirection</Name>
                              <Value>ATXRouteCardRouteTmp.OprIdBarCode</Value>
                            </CustomProperty>
                          </CustomProperties>
                          <Style>
                            <Border>
                              <Color>LightGrey</Color>
                              <Style>Solid</Style>
                            </Border>
                            <PaddingLeft>2pt</PaddingLeft>
                            <PaddingRight>2pt</PaddingRight>
                            <PaddingTop>2pt</PaddingTop>
                            <PaddingBottom>2pt</PaddingBottom>
                          </Style>
                        </Textbox>
                      </CellContents>
                    </TablixCell>
                  </TablixCells>
                </TablixRow>
              </TablixRows>
            </TablixBody>
            <TablixColumnHierarchy>
              <TablixMembers>
                <TablixMember />
                <TablixMember />
                <TablixMember />
                <TablixMember />
              </TablixMembers>
            </TablixColumnHierarchy>
            <TablixRowHierarchy>
              <TablixMembers>
                <TablixMember>
                  <KeepWithGroup>After</KeepWithGroup>
                </TablixMember>
                <TablixMember>
                  <Group Name="Details" />
                </TablixMember>
              </TablixMembers>
            </TablixRowHierarchy>
            <DataSetName>Route</DataSetName>
            <Top>0.77083in</Top>
            <Left>0.2175in</Left>
            <Height>0.5in</Height>
            <Width>7.46528in</Width>
            <ZIndex>1</ZIndex>
            <Style>
              <Border>
                <Style>None</Style>
              </Border>
            </Style>
          </Tablix>
        </ReportItems>
        <Height>1.40625in</Height>
        <Style />
      </Body>
      <Width>7.89583in</Width>
      <Page>
        <PageHeader>
          <Height>2.155in</Height>
          <PrintOnFirstPage>true</PrintOnFirstPage>
          <PrintOnLastPage>true</PrintOnLastPage>
          <ReportItems>
            <Textbox Name="Textbox1">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=Labels!@ATXAT:NewLabel216</Value>
                      <Style>
                        <FontWeight>Bold</FontWeight>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style>
                    <TextAlign>Left</TextAlign>
                  </Style>
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.13417in</Top>
              <Left>0.2175in</Left>
              <Height>0.19792in</Height>
              <Width>3.64583in</Width>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Textbox Name="Textbox2">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=First(Fields!ProdIdBarcode.Value, "Header")</Value>
                      <Style>
                        <FontFamily>BC CBar 3 to 1 Narrow</FontFamily>
                        <FontSize>30pt</FontSize>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style>
                    <TextAlign>Right</TextAlign>
                  </Style>
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox2</rd:DefaultName>
              <Top>0.13417in</Top>
              <Left>4.00917in</Left>
              <Height>0.36875in</Height>
              <Width>3.63541in</Width>
              <ZIndex>1</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
                <PaddingLeft>2pt</PaddingLeft>
                <PaddingRight>2pt</PaddingRight>
                <PaddingTop>2pt</PaddingTop>
                <PaddingBottom>2pt</PaddingBottom>
              </Style>
            </Textbox>
            <Textbox Name="Textbox3">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=First(Fields!ProdId.Value, "Header")</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                        <FontWeight>Bold</FontWeight>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style />
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.34667in</Top>
              <Left>0.51264in</Left>
              <Height>0.15625in</Height>
              <Width>0.8507in</Width>
              <ZIndex>2</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Textbox Name="Textbox4">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=Format("dd/mm/yyy", today())</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                        <FontWeight>Bold</FontWeight>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style>
                    <TextAlign>Left</TextAlign>
                  </Style>
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.34667in</Top>
              <Left>1.37167in</Left>
              <Height>0.15625in</Height>
              <Width>1.10416in</Width>
              <ZIndex>3</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Textbox Name="Textbox5">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=Labels!@ATXAT:NewLabel219</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                        <FontWeight>Bold</FontWeight>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style />
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.5875in</Top>
              <Left>0.2175in</Left>
              <Height>0.15625in</Height>
              <Width>3.64583in</Width>
              <ZIndex>4</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Textbox Name="Textbox6">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=First(Fields!CustName.Value, "Header")</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style />
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.7625in</Top>
              <Left>0.2175in</Left>
              <Height>0.16667in</Height>
              <Width>3.64583in</Width>
              <ZIndex>5</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Textbox Name="Textbox7">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=Labels!@ATXAT:NewLabel218</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                        <FontWeight>Bold</FontWeight>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style>
                    <TextAlign>Right</TextAlign>
                  </Style>
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.5875in</Top>
              <Left>5.97792in</Left>
              <Height>0.15625in</Height>
              <Width>1.66666in</Width>
              <ZIndex>6</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Textbox Name="Textbox8">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=Sum(Fields!Qty.Value, "Breakdown")</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                        <Format>#,0.00;-#,0.00;'0.00'</Format>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style>
                    <TextAlign>Right</TextAlign>
                  </Style>
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.7625in</Top>
              <Left>5.97792in</Left>
              <Height>0.16667in</Height>
              <Width>1.66666in</Width>
              <ZIndex>7</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
            <Rectangle Name="Rectangle1">
              <ReportItems>
                <Textbox Name="Textbox10">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel220</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.05958in</Top>
                  <Left>0.0625in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox11">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!CustPurchaseOrder.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.22625in</Top>
                  <Left>0.0625in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>1</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox13">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!ItemId.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.22625in</Top>
                  <Left>1.4375in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.75in</Width>
                  <ZIndex>2</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox12">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel221</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.05958in</Top>
                  <Left>1.4375in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.75in</Width>
                  <ZIndex>3</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox14">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel222</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.05958in</Top>
                  <Left>3.1875in</Left>
                  <Height>0.16667in</Height>
                  <Width>3.19722in</Width>
                  <ZIndex>4</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox15">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!ItemName.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.22625in</Top>
                  <Left>3.1875in</Left>
                  <Height>0.16667in</Height>
                  <Width>3.19722in</Width>
                  <ZIndex>5</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox16">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel223</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.05958in</Top>
                  <Left>6.40278in</Left>
                  <Height>0.16667in</Height>
                  <Width>1in</Width>
                  <ZIndex>6</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox17">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!SalesId.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.22625in</Top>
                  <Left>6.40278in</Left>
                  <Height>0.16667in</Height>
                  <Width>1in</Width>
                  <ZIndex>7</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Line Name="Line1">
                  <Top>0.52083in</Top>
                  <Height>0in</Height>
                  <Width>7.46528in</Width>
                  <ZIndex>8</ZIndex>
                  <Style>
                    <Border>
                      <Style>Solid</Style>
                    </Border>
                  </Style>
                </Line>
                <Textbox Name="Textbox18">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel224</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.54861in</Top>
                  <Left>0.0625in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>9</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox19">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!InventBatchId.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.71528in</Top>
                  <Left>0.0625in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>10</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox20">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel225</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.54861in</Top>
                  <Left>1.4375in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>11</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox21">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!SeasonId.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.71528in</Top>
                  <Left>1.4375in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>12</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox22">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=Labels!@ATXAT:NewLabel226</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                            <FontWeight>Bold</FontWeight>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.54861in</Top>
                  <Left>2.82639in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>13</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
                <Textbox Name="Textbox23">
                  <CanGrow>true</CanGrow>
                  <KeepTogether>true</KeepTogether>
                  <Paragraphs>
                    <Paragraph>
                      <TextRuns>
                        <TextRun>
                          <Value>=First(Fields!DestinationPlaceId.Value, "Header")</Value>
                          <Style>
                            <FontSize>9pt</FontSize>
                          </Style>
                        </TextRun>
                      </TextRuns>
                      <Style />
                    </Paragraph>
                  </Paragraphs>
                  <rd:DefaultName>Textbox10</rd:DefaultName>
                  <Top>0.71528in</Top>
                  <Left>2.82639in</Left>
                  <Height>0.16667in</Height>
                  <Width>1.375in</Width>
                  <ZIndex>14</ZIndex>
                  <Style>
                    <Border>
                      <Style>None</Style>
                    </Border>
                  </Style>
                </Textbox>
              </ReportItems>
              <KeepTogether>true</KeepTogether>
              <Top>1.05708in</Top>
              <Left>0.2175in</Left>
              <Height>1in</Height>
              <Width>7.46528in</Width>
              <ZIndex>8</ZIndex>
              <Style>
                <Border>
                  <Style>Solid</Style>
                </Border>
              </Style>
            </Rectangle>
            <Textbox Name="Textbox9">
              <CanGrow>true</CanGrow>
              <KeepTogether>true</KeepTogether>
              <Paragraphs>
                <Paragraph>
                  <TextRuns>
                    <TextRun>
                      <Value>=Labels!@ATXAT:NewLabel217</Value>
                      <Style>
                        <FontSize>9pt</FontSize>
                        <FontWeight>Bold</FontWeight>
                      </Style>
                    </TextRun>
                  </TextRuns>
                  <Style />
                </Paragraph>
              </Paragraphs>
              <rd:DefaultName>Textbox1</rd:DefaultName>
              <Top>0.34667in</Top>
              <Left>0.2175in</Left>
              <Height>0.15625in</Height>
              <Width>0.28125in</Width>
              <ZIndex>9</ZIndex>
              <Style>
                <Border>
                  <Style>None</Style>
                </Border>
              </Style>
            </Textbox>
          </ReportItems>
          <Style>
            <Border>
              <Style>None</Style>
            </Border>
          </Style>
        </PageHeader>
        <InteractiveHeight>11in</InteractiveHeight>
        <InteractiveWidth>8.5in</InteractiveWidth>
        <LeftMargin>0.25in</LeftMargin>
        <RightMargin>0.25in</RightMargin>
        <TopMargin>0.25in</TopMargin>
        <BottomMargin>0.25in</BottomMargin>
        <Style />
      </Page>
    </ReportSection>
  </ReportSections>
  <ReportParameters>
    <ReportParameter Name="AX_PartitionKey">
      <DataType>String</DataType>
      <Nullable>true</Nullable>
      <AllowBlank>true</AllowBlank>
      <Prompt>AX_PartitionKey</Prompt>
      <Hidden>true</Hidden>
    </ReportParameter>
    <ReportParameter Name="AX_CompanyName">
      <DataType>String</DataType>
      <Prompt>AX_CompanyName</Prompt>
      <Hidden>true</Hidden>
    </ReportParameter>
    <ReportParameter Name="AX_UserContext">
      <DataType>String</DataType>
      <Nullable>true</Nullable>
      <AllowBlank>true</AllowBlank>
      <Prompt>AX_UserContext</Prompt>
      <Hidden>true</Hidden>
    </ReportParameter>
    <ReportParameter Name="AX_RenderingCulture">
      <DataType>String</DataType>
      <Nullable>true</Nullable>
      <AllowBlank>true</AllowBlank>
      <Prompt>AX_RenderingCulture</Prompt>
      <Hidden>true</Hidden>
    </ReportParameter>
    <ReportParameter Name="AX_ReportContext">
      <DataType>String</DataType>
      <Nullable>true</Nullable>
      <AllowBlank>true</AllowBlank>
      <Prompt>AX_ReportContext</Prompt>
      <Hidden>true</Hidden>
      <UsedInQuery>True</UsedInQuery>
    </ReportParameter>
    <ReportParameter Name="AX_RdpPreProcessedId">
      <DataType>String</DataType>
      <Nullable>true</Nullable>
      <AllowBlank>true</AllowBlank>
      <Prompt>AX_RdpPreProcessedId</Prompt>
      <Hidden>true</Hidden>
    </ReportParameter>
    <ReportParameter Name="Header_RecId">
      <DataType>String</DataType>
      <Prompt>Header_RecId</Prompt>
      <Hidden>true</Hidden>
    </ReportParameter>
    <ReportParameter Name="Header_RouteOprId">
      <DataType>String</DataType>
      <Prompt>Header_RouteOprId</Prompt>
    </ReportParameter>
  </ReportParameters>
  <Language>en-US</Language>
  <rd:ReportUnitType>Inch</rd:ReportUnitType>
  <rd:ExpressionDialog>Microsoft.Dynamics.Framework.Design.Reports.ExpressionEditor.ExpressionEditorDialog, Microsoft.Dynamics.Framework.Design.Reports</rd:ExpressionDialog>
  <rd:ReportID>f1e435ea-b716-4c60-8e53-bcd0144c1854</rd:ReportID>
</Report>�ATXRouteCard�