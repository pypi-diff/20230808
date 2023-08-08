# Comparing `tmp/sapiopylib-2023.6.8.142.tar.gz` & `tmp/sapiopylib-2023.8.8.149.tar.gz`

## Comparing `sapiopylib-2023.6.8.142.tar` & `sapiopylib-2023.8.8.149.tar`

### file list

```diff
@@ -1,100 +1,102 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/MessengerService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Message.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25176 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/LICENSE
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/pyproject.toml
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41145 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0    11574 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25176 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    58080 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55252 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    23360 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25753 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46635 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/src/sapiopylib/utils/string.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/LICENSE
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/README.md
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/pyproject.toml
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 sapiopylib-2023.8.8.149/PKG-INFO
```

### Comparing `sapiopylib-2023.6.8.142/INSTALL.md` & `sapiopylib-2023.8.8.149/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from enum import Enum
 from typing import Dict, Any, Optional, Type, List
 
 
 class CspDataException(Exception):
     """
     This is thrown when there is anything explicitly wrong detected while converting CSP data in Python.
     """
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
-from typing import Optional, List, Dict
 
-from sapiopylib.csp.data.PyCspFieldMap import PyCspObject, CspDataException
-from sapiopylib.csp.data.plotly.PlotlyCspEnums import *
 import re
 from re import Pattern, Match
+from typing import List, Dict
+
+from sapiopylib.csp.data.PyCspFieldMap import PyCspObject, CspDataException
+from sapiopylib.csp.data.plotly.PlotlyCspEnums import *
 
 
 class PlotlyColor:
     """
     Construct a plotly color object to produce color strings used by plotly attribute in a UI color property.
     """
     red: int
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseTraceType
-from plotly.graph_objs import Figure, Layout, Scatter, Bar, Box, Heatmap, Histogram, Densitymapbox, Histogram2dContour
+from plotly.graph_objs import Figure, Layout, Scatter, Bar, Box, Heatmap, Histogram, Histogram2dContour
 from plotly.graph_objs.layout import Margin, XAxis, YAxis
 
 from sapiopylib.csp.data.plotly.PlotlyCspData import *
 
 
 def _get_plotly_marker(csp_marker: Optional[PlotlyCspMarker]):
     if csp_marker is None:
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataMgmtService.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from sapiopylib.rest.DashboardManager import DashboardManager
+from sapiopylib.rest.DataService import DataManager
 from sapiopylib.rest.DataTypeService import DataTypeManager
 
 from sapiopylib.rest.AccessionService import AccessionManager
 from sapiopylib.rest.CustomReportService import CustomReportManager
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 from sapiopylib.rest.ELNService import ElnManager
 from sapiopylib.rest.GroupManagerService import VeloxGroupManager
@@ -86,7 +87,14 @@
         Get the group manager that contains info about groups and user memberships into groups.
         """
         return VeloxGroupManager(user)
 
     @staticmethod
     def get_messenger(user: SapioUser) -> SapioMessenger:
         return SapioMessenger(user)
+
+    @staticmethod
+    def get_data_manager(user: SapioUser) -> DataManager:
+        """
+        Get the data manager that helps import/export data from and to a file.
+        """
+        return DataManager(user)
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,15 @@
         :param record: The record to obtain attachment data from.
         :param data_sink: The data sink method to consume data stream
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/attachment/' + urllib.parse.quote(data_type_name) + "/" + \
                    urllib.parse.quote(str(record_id))
-        self.user.consume_record_attachment_data(sub_path, data_sink)
+        self.user.consume_octet_stream_get(sub_path, data_sink)
 
     def set_record_image(self, record: DataRecord,
                          data_stream: IO) -> None:
         """
         Set the record image on the record defined by the data type name and record ID parameters.
         :param record: The record to set image for.
         :param data_stream: The stream to be consumed as upload image data.
@@ -437,15 +437,15 @@
         Get the data record image and consume it with data sink.
         :param record: The record to get image from.
         :param data_sink: The data sink to consume image data.
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/image/' + urllib.parse.quote(data_type_name) + "/" + urllib.parse.quote(str(record_id))
-        self.user.consume_record_attachment_data(sub_path, data_sink)
+        self.user.consume_octet_stream_get(sub_path, data_sink)
 
     def delete_data_record(self, record: DataRecord, recursive_delete: bool = False) -> None:
         """
         Delete a single data record from Sapio.
         :param record: The record to be deleted.
         :param recursive_delete: Whether we will delete the record's descendants if there is no other lineage.
         """
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/MessengerService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/MessengerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/User.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/User.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,28 +163,43 @@
                              timeout=self.timeout_seconds)
 
     def get(self, url_sub_path: str, params: Optional[dict] = None) -> Response:
         return requests.get(self.url + url_sub_path, params=params,
                             headers=self.get_http_headers(), verify=self.verify_ssl_cert,
                             timeout=self.timeout_seconds)
 
-    def consume_record_attachment_data(self, url_sub_path: str,
-                                       data_sink: Callable[[bytes], None],
-                                       params: Optional[dict] = None,
-                                       chunk_size=1024 * 1024) -> None:
+    def consume_octet_stream_get(self, url_sub_path: str,
+                                 data_sink: Callable[[bytes], None],
+                                 params: Optional[dict] = None,
+                                 chunk_size=1024 * 1024) -> None:
         session = requests.Session()
         url = self.url + url_sub_path
         headers = self.get_http_headers()
         response = session.get(url=url, params=params,
                                headers=headers, verify=self.verify_ssl_cert,
                                timeout=self.timeout_seconds, stream=True)
         self.raise_for_status(response)
         for chunk in response.iter_content(chunk_size=chunk_size):
             data_sink(chunk)
 
+    def consume_octet_stream_post(self, url_sub_path: str,
+                                  data_sink: Callable[[bytes], None],
+                                  params: Optional[dict] = None,
+                                  payload = None,
+                                  chunk_size=1024 * 1024) -> None:
+        session = requests.Session()
+        url = self.url + url_sub_path
+        headers = self.get_http_headers()
+        response = session.post(url=url, params=params, json=payload,
+                                headers=headers, verify=self.verify_ssl_cert,
+                                timeout=self.timeout_seconds, stream=True)
+        self.raise_for_status(response)
+        for chunk in response.iter_content(chunk_size=chunk_size):
+            data_sink(chunk)
+
     def delete(self, url_sub_path: str, params: Optional[dict] = None, payload=None) -> Response:
         return requests.delete(self.url + url_sub_path, params=params, json=payload,
                                headers=self.get_http_headers(), verify=self.verify_ssl_cert,
                                timeout=self.timeout_seconds)
 
     def put(self, url_sub_path: str, params: Optional[dict] = None, payload=None) -> Response:
         return requests.put(self.url + url_sub_path, params=params, json=payload,
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/WebhookService.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                                                                                self.verify_sapio_cert)
         # noinspection PyBroadException
         try:
             return self.run(context).to_json()
         except Exception:
             print('Error occurred while running webhook custom logic. See traceback.', file=sys.stderr)
             traceback.print_exc()
-            return SapioWebhookResult(False).to_json()
+            return SapioWebhookResult(False, display_text="Error occurred during webhook execution.").to_json()
 
     @abstractmethod
     def run(self, context: SapioWebhookContext) -> SapioWebhookResult:
         """
         The execution details for this service.
         :param context: The webhook context provided to you when it is called.
         :return: The webhook result to send back to Sapio.
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Message.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/Message.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,19 @@
         return hash((self.form_name, self.data_field_name, self.order))
 
     def __lt__(self, other):
         if other is None:
             return False
         if not isinstance(other, FieldDefinitionPosition):
             return False
-        return (self.order, self.form_column, self.data_field_name) < \
-            (other.order, other.form_column, other.data_field_name)
+        if self.order != other.order:
+            return self.order < other.order
+        if self.form_column != other.form_column:
+            return self.form_column < other.form_column
+        return self.data_field_name < other.data_field_name
 
     def __init__(self, data_field_name: str,
                  form_name: Optional[str] = None, order: Optional[int] = None, form_column: Optional[int] = None,
                  form_column_span: Optional[int] = None, field_height: Optional[int] = None):
         self.form_name = form_name
         self.data_field_name = data_field_name
         self.order = order
@@ -337,16 +340,21 @@
         return self.component_name == other.component_name
 
     def __lt__(self, other):
         if other is None:
             return False
         if not isinstance(other, AbstractDataTypeComponent):
             return False
-        return (self.order, self.column, self.display_name, self.component_name) < \
-            (other.order, other.column, other.display_name, other.component_name)
+        if self.order != other.order:
+            return self.order < other.order
+        if self.column != other.column:
+            return self.column < other.column
+        if self.display_name != other.display_name:
+            return self.display_name < other.display_name
+        return self.component_name < other.component_name
 
     @abstractmethod
     def get_layout_component_type(self) -> DataTypeLayoutComponentTypes:
         pass
 
     def to_pojo(self) -> Dict[str, Any]:
         ret: dict = {
@@ -425,16 +433,19 @@
             self.tab_name == other.tab_name
 
     def __le__(self, other):
         if other is None:
             return False
         if not isinstance(other, DataTypeComponentTabDefinition):
             return False
-        return (self.tab_order, self.tab_display_name, self.tab_name) < \
-            (other.tab_order, other.tab_display_name, other.tab_name)
+        if self.tab_order != other.tab_order:
+            return self.tab_order < other.tab_order
+        if self.tab_display_name != other.tab_display_name:
+            return self.tab_display_name < other.tab_display_name
+        return self.tab_name != other.tab_name
 
     def __str__(self):
         return self.tab_display_name
 
 
 def _parse_data_type_component_tab_def(json_dct: Dict[str, Any]) -> DataTypeComponentTabDefinition:
     tab_name: str = json_dct.get('tabName')
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,19 @@
                (other.tab_order, other.tab_display_name, other.tab_name)
 
     def __le__(self, other):
         if other is None:
             return False
         if not isinstance(other, DataTypeOuterTabDefinition):
             return False
-        return (self.tab_order, self.tab_display_name, self.tab_name) < \
-               (other.tab_order, other.tab_display_name, other.tab_name)
+        if self.tab_order != other.tab_order:
+            return self.tab_order < other.tab_order
+        if self.tab_display_name != other.tab_display_name:
+            return self.tab_display_name < other.tab_display_name
+        return self.tab_name < other.tab_name
 
     def __str__(self):
         return self.tab_display_name
 
 
 def _parse_outer_tab_definition(json_dct: Dict[str, Any]) -> DataTypeOuterTabDefinition:
     layout_component_pojo_map: Dict[str, Dict[str, Any]] = json_dct.get('layoutComponentMap')
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Any, List, Optional
 from abc import abstractmethod, ABC
 from enum import Enum
 
 from sapiopylib.rest.pojo.Sort import SortDirection, SortDirectionParser
+import sapiopylib.utils.string as ssutil
 
 
 class FieldType(Enum):
     """
     All possible data field types in a data field of any data type.
     """
     BOOLEAN = 0, "True / False", True
@@ -1063,21 +1064,21 @@
     unique_value: bool = json_dct.get('uniqueValue')
     multi_select: bool = json_dct.get('multiSelect')
     list_mode: ListMode
     list_name: Optional[str] = None
     report_name: Optional[str] = None
     plugin_name: Optional[str] = None
     if list_mode_str.startswith(ListMode.LIST.list_mode_name):
-        list_name = list_mode_str.removeprefix(ListMode.LIST.list_mode_name)
+        list_name = ssutil.removeprefix(list_mode_str, ListMode.LIST.list_mode_name)
         list_mode = ListMode.LIST
     elif list_mode_str.startswith(ListMode.REPORT.list_mode_name):
-        report_name = list_mode_str.removeprefix(ListMode.REPORT.list_mode_name)
+        report_name =  ssutil.removeprefix(list_mode_str, ListMode.REPORT.list_mode_name)
         list_mode = ListMode.REPORT
     elif list_mode_str.startswith(ListMode.PLUGIN.list_mode_name):
-        plugin_name = list_mode_str.removeprefix(ListMode.PLUGIN.list_mode_name)
+        plugin_name =  ssutil.removeprefix(list_mode_str, ListMode.PLUGIN.list_mode_name)
         list_mode = ListMode.PLUGIN
     elif list_mode_str.startswith(ListMode.USER_GROUP.list_mode_name):
         list_mode = ListMode.USER_GROUP
     elif list_mode_str.startswith(ListMode.NON_API_USER.list_mode_name):
         list_mode = ListMode.NON_API_USER
     elif list_mode_str.startswith(ListMode.USER.list_mode_name):
         list_mode = ListMode.USER
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         if self.dashboard_guid is not None:
             ret['dashboardGuid'] = self.dashboard_guid
         if self.data_source_entry_id is not None:
             ret['dataSourceEntryId'] = self.data_source_entry_id
         return ret
 
 
-class ELNFormEntryUpdateCriteria(AbstractElnEntryUpdateCriteria):
+class ElnFormEntryUpdateCriteria(AbstractElnEntryUpdateCriteria):
     """
     Form Entry Update Request payload data.
     Create this payload object and set the attributes you want to update before sending the request.
     """
     form_name_list: Optional[List[str]]
     data_type_layout_name: Optional[str]
     record_id: Optional[int]
@@ -448,15 +448,15 @@
         """
         entry_update_criteria: AbstractElnEntryUpdateCriteria
         if entry.entry_type == ElnEntryType.Attachment:
             entry_update_criteria = ElnAttachmentEntryUpdateCriteria()
         elif entry.entry_type == ElnEntryType.Dashboard:
             entry_update_criteria = ElnDashboardEntryUpdateCriteria()
         elif entry.entry_type == ElnEntryType.Form:
-            entry_update_criteria = ELNFormEntryUpdateCriteria()
+            entry_update_criteria = ElnFormEntryUpdateCriteria()
         elif entry.entry_type == ElnEntryType.Plugin:
             entry_update_criteria = ElnPluginEntryUpdateCriteria()
         elif entry.entry_type == ElnEntryType.Table:
             entry_update_criteria = ElnTableEntryUpdateCriteria()
         elif entry.entry_type == ElnEntryType.TempData:
             entry_update_criteria = ElnTempDataEntryUpdateCriteria()
         elif entry.entry_type == ElnEntryType.Text:
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 from abc import ABC, abstractmethod
 from typing import Any, List, Dict, Optional
 
+from sapiopylib.rest.pojo.datatype.FieldDefinition import AbstractVeloxFieldDefinition
 from sapiopylib.rest.pojo.datatype.TemporaryDataType import TemporaryDataType
 from sapiopylib.rest.pojo.webhook.WebhookEnums import CallbackType
 
 
 class AbstractClientCallbackRequest(ABC):
     """
     A request for a client callback to be shown to the user that invoked the webhook.
@@ -20,14 +21,50 @@
 
     def to_json(self) -> Dict[str, Any]:
         return {
             'callbackType': self.get_callback_type().name
         }
 
 
+class DataRecordSelectionRequest(AbstractClientCallbackRequest):
+    """
+    A callback request to select a list of field map rows.
+    """
+    data_type_display_name: str
+    data_type_plural_display_name: str
+    field_def_list: List[AbstractVeloxFieldDefinition]
+    field_map_list: List[Dict[str, Any]]
+    dialog_message: Optional[str]
+    multi_select: bool
+
+    def __init__(self, data_type_display_name: str, data_type_plural_display_name: str,
+                 field_def_list: List[AbstractVeloxFieldDefinition],
+                 field_map_list: List[Dict[str, Any]],
+                 dialog_message: Optional[str] = None, multi_select: bool = False):
+        self.data_type_display_name = data_type_display_name
+        self.data_type_plural_display_name = data_type_plural_display_name
+        self.field_def_list = field_def_list
+        self.field_map_list = field_map_list
+        self.dialog_message = dialog_message
+        self.multi_select = multi_select
+
+    def get_callback_type(self) -> CallbackType:
+        return CallbackType.DATA_RECORD_SELECTION
+
+    def to_json(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = super().to_json()
+        ret['dialogMessage'] = self.dialog_message
+        ret['dataTypeDisplayName'] = self.data_type_display_name
+        ret['dataTypePluralDisplayName'] = self.data_type_plural_display_name
+        ret['fieldDefinitionList'] = [x.to_json() for x in self.field_def_list]
+        ret['fieldMapList'] = self.field_map_list
+        ret['multiSelect'] = self.multi_select
+        return ret
+
+
 class MultiFilePromptRequest(AbstractClientCallbackRequest):
     """
     Request the user to upload multiple files. User will be asked fo upload one or more files.
     """
     dialog_title: str
     show_image_editor: bool
     file_extension: Optional[str]
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             return FormEntryDialogResult(user_cancelled, user_response_map=user_response_map)
         elif callback_type == CallbackType.LIST_DIALOG:
             selected_options_list: Optional[List[str]] = json_dct.get('selectedOptionList')
             return ListDialogResult(user_cancelled, selected_options_list=selected_options_list)
         elif callback_type == CallbackType.OPTION_DIALOG:
             selection: Optional[int] = json_dct.get('selection')
             button_text: Optional[str] = json_dct.get('buttonText')
-            return OptionDialogResult(user_cancelled, selection == selection, button_text=button_text)
+            return OptionDialogResult(user_cancelled, selection=selection, button_text=button_text)
         elif callback_type == CallbackType.TABLE_ENTRY_DIALOG:
             user_response_data_list: Optional[List[Dict[str, Any]]] = \
                 json_dct.get('userResponseDataList')
             return TableEntryDialogResult(user_cancelled, user_response_data_list=user_response_data_list)
         elif callback_type == CallbackType.WRITE_FILE:
             return WriteFileResult(user_cancelled)
         else:
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sapiopylib.rest.pojo.chartdata.DashboardDefinition import BarLineChartDefinition, DashboardDefinition, \
     XyChartDefinition, HeatMapChartDefinition, GanttChartDefinition
 from sapiopylib.rest.pojo.chartdata.DashboardEnums import ChartGroupingType, \
     ChartOperationType, DashboardScope, PointShapeType, LineStyleType
 from sapiopylib.rest.pojo.chartdata.DashboardSeries import BarChartSeries, XyChartSeries, HeatMapChartSeries, \
     GanttChartSeries
 from sapiopylib.rest.pojo.eln.ExperimentEntry import ExperimentEntry
-from sapiopylib.rest.pojo.eln.ExperimentEntryCriteria import ElnEntryCriteria, ELNFormEntryUpdateCriteria, \
+from sapiopylib.rest.pojo.eln.ExperimentEntryCriteria import ElnEntryCriteria, ElnFormEntryUpdateCriteria, \
     ElnPluginEntryUpdateCriteria, ElnDashboardEntryUpdateCriteria
 from sapiopylib.rest.pojo.eln.SapioELNEnums import ElnEntryType, ElnBaseDataType
 from sapiopylib.rest.utils.Protocols import ElnExperimentProtocol, ElnEntryStep
 from sapiopylib.rest.utils.plates.MultiLayerPlating import MultiLayerPlateConfig, MultiLayerPlateLayer
 from sapiopylib.rest.utils.plates.MultiLayerPlatingUtils import MultiLayerPlatingManager
 
 
@@ -72,15 +72,15 @@
         :param initial_attached_record: The initially attached record for the new form step.
         Note: if unspecified, a form step will use a new record.
         :return: The new form step.
         """
         eln_manager, new_entry = _get_entry_creation_criteria(data_type_name, protocol, step_name, ElnEntryType.Form)
         if initial_attached_record:
             validate_records_is_of_type(data_type_name, [initial_attached_record])
-            update_criteria = ELNFormEntryUpdateCriteria()
+            update_criteria = ElnFormEntryUpdateCriteria()
             update_criteria.record_id = initial_attached_record.get_record_id()
             eln_manager.update_experiment_entry(protocol.eln_experiment.notebook_experiment_id, new_entry.entry_id,
                                                 update_criteria)
         ret = ElnEntryStep(protocol, new_entry)
         protocol.invalidate()
         return ret
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/Protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 from sapiopylib.rest.pojo.eln.ExperimentEntry import ExperimentEntry
 
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 
 from sapiopylib.rest.pojo.DataRecordPaging import DataRecordPojoPageCriteria
 
-from sapiopylib.rest.pojo.eln.ExperimentEntryCriteria import ExperimentEntryCriteriaUtil
+from sapiopylib.rest.pojo.eln.ExperimentEntryCriteria import ExperimentEntryCriteriaUtil, \
+    ElnAttachmentEntryUpdateCriteria, AbstractElnEntryUpdateCriteria, ElnFormEntryUpdateCriteria
 
-from sapiopylib.rest.pojo.eln.SapioELNEnums import ElnExperimentStatus, ExperimentEntryStatus, ElnBaseDataType
+from sapiopylib.rest.pojo.eln.SapioELNEnums import ElnExperimentStatus, ExperimentEntryStatus, ElnBaseDataType, \
+    ElnEntryType
 
 from sapiopylib.rest.DataMgmtService import DataMgmtServer
 
 from sapiopylib.rest.User import SapioUser
 
 from sapiopylib.rest.pojo.eln.ElnExperiment import ElnExperiment, ElnExperimentUpdateCriteria
 
@@ -45,14 +47,41 @@
         pass
 
     @abstractmethod
     def get_data_type_names(self) -> List[str]:
         pass
 
     @abstractmethod
+    def add_records(self, records_to_add: List[DataRecord]):
+        """
+        Add records to the current step.
+        Throws an error if this operation is not supported.
+        For ELN entry, only table entry steps can use this method.
+        """
+        pass
+
+    @abstractmethod
+    def remove_records(self, records_to_remove: List[DataRecord]):
+        """
+        Remove records from the current step.
+        Throws an error if this operation is not supported.
+        For ELN entry, only table entry steps can use this method.
+        """
+        pass
+
+    @abstractmethod
+    def set_records(self, records_to_set: List[DataRecord]):
+        """
+        Set records on the current step.
+        Available for form, attachment, and table entries.
+        However, for form and attachment, exactly one record must be specified here.
+        """
+        pass
+
+    @abstractmethod
     def get_records(self) -> List[DataRecord]:
         pass
 
     @abstractmethod
     def get_options(self) -> Dict[str, str]:
         pass
 
@@ -328,14 +357,67 @@
         return self.eln_entry.entry_id
 
     def get_data_type_names(self) -> List[str]:
         if self.eln_entry.data_type_name:
             return [self.eln_entry.data_type_name]
         return []
 
+    def add_records(self, records_to_add: List[DataRecord]):
+        if not records_to_add:
+            return
+        eln_manager = DataMgmtServer.get_eln_manager(self.user)
+        if self.eln_entry.entry_type != ElnEntryType.Table:
+            raise ValueError("ELN experiment entry must be a table entry when adding records to ELN step.")
+        eln_manager.add_records_to_table_entry(self.protocol.eln_experiment.notebook_experiment_id,
+                                               self.eln_entry.entry_id, records_to_add)
+
+    def remove_records(self, records_to_remove: List[DataRecord]):
+        if not records_to_remove:
+            return
+        eln_manager = DataMgmtServer.get_eln_manager(self.user)
+        if self.eln_entry.entry_type != ElnEntryType.Table:
+            raise ValueError("ELN experiment entry must be a table entry when removing records to ELN step.")
+        eln_manager.remove_records_from_table_entry(self.protocol.eln_experiment.notebook_experiment_id,
+                                                    self.eln_entry.entry_id, [x.record_id for x in records_to_remove])
+
+    def set_records(self, records_to_set: List[DataRecord]):
+        eln_manager = DataMgmtServer.get_eln_manager(self.user)
+        if self.eln_entry.entry_type == ElnEntryType.Table:
+            cur_records = self.get_records()
+            cur_record_id_set = [x.record_id for x in cur_records]
+            record_id_to_set = [x.record_id for x in records_to_set]
+            records_to_add: List[DataRecord] = []
+            records_to_remove: List[DataRecord] = []
+            for record_to_set in records_to_set:
+                if record_to_set.record_id not in cur_record_id_set:
+                    records_to_add.append(record_to_set)
+            for cur_record in cur_records:
+                if cur_record.record_id not in record_id_to_set:
+                    records_to_remove.append(cur_record)
+            if records_to_add:
+                self.add_records(records_to_add)
+            if records_to_remove:
+                self.remove_records(records_to_remove)
+        elif self.eln_entry.entry_type in [ElnEntryType.Form, ElnEntryType.Attachment]:
+            if len(records_to_set) != 1:
+                raise ValueError("For form and attachments, there must be exactly one backing record.")
+            record_id_to_set = records_to_set[0].record_id
+            criteria: AbstractElnEntryUpdateCriteria
+            if self.eln_entry.entry_type == ElnEntryType.Attachment:
+                criteria = ElnAttachmentEntryUpdateCriteria()
+                criteria.record_id = record_id_to_set
+                criteria.attachment_name = records_to_set[0].get_field_value("FilePath")
+            else:
+                criteria = ElnFormEntryUpdateCriteria()
+                criteria.record_id = record_id_to_set
+            eln_manager.update_experiment_entry(self.protocol.eln_experiment.notebook_experiment_id,
+                                                self.eln_entry.entry_id, criteria)
+        else:
+            raise ValueError("The entry type does not support set records operation.")
+
     def get_records(self) -> List[DataRecord]:
         eln_manager = DataMgmtServer.get_eln_manager(self.user)
         has_more_pages: bool = True
         next_page_criteria: Optional[DataRecordPojoPageCriteria] = None
         ret = []
         while has_more_pages:
             page_result = eln_manager.get_data_records_for_entry(self.protocol.get_id(), self.get_id(),
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,29 +78,31 @@
         self._model_fields[field_name] = field_value
 
     def get(self, field_name: str):
         """
         Get the value by a field name in this record model.
         Return None if this field does not exist.
         """
+        if field_name and "RecordId".lower() == field_name.lower():
+            return self._model.record_id
         return self._model_fields.get(field_name)
 
     def __setitem__(self, field_name: str, field_value: Any):
         old_value = self._model_fields.get(field_name)
         if old_value == field_value:
             return
         self._model_fields[field_name] = field_value
         from sapiopylib.rest.utils.recordmodel.RecordModelEvents import FieldChangeEvent
         self._model.record_model_manager.event_bus.fire_field_change_event(FieldChangeEvent(
             self._model, field_name, old_value, field_value))
         # Handle for side links.
         dt_cache_man: DataTypeCacheManager = self._model.record_model_manager.data_type_cache_manager
         if dt_cache_man.is_side_link_field(self._model.data_type_name, field_name):
             if field_value is None:
-                self._model.record_model_manager.event_bus.fire_side_link_changed_event(self, field_name, None)
+                self._model.record_model_manager.event_bus.fire_side_link_changed_event(self._model, field_name, None)
             else:
                 target_record_id: int = int(field_value)
                 self._model.record_model_manager.event_bus.fire_side_link_changed_event(self._model,
                                                                                         field_name, target_record_id)
 
     def __delitem__(self, field_name: str):
         if field_name not in self._model_fields:
@@ -141,14 +143,15 @@
 class PyRecordModel:
     """
     A record model instance that is backed by a data record.
     """
     _backing_record: DataRecord
     _model_fields: RecordModelFieldMap
     __is_deleted: bool
+    __object_id: int
 
     _children_types_loaded: Set[str]
     _parent_types_loaded: Set[str]
     _children_models_by_type: SetMultimap[str, PyRecordModel]
     _parent_models_by_type: SetMultimap[str, PyRecordModel]
     _forward_side_link_cache: Dict[str, Optional[int]]
     _loaded_forward_side_link_field_names: Set[str]
@@ -176,17 +179,18 @@
         self._loaded_forward_side_link_field_names = set()
         self._reverse_side_link_cache = SetMultimap()
         self._loaded_reverse_side_links = set()
         self._non_loaded_removed_parents = set()
         self._non_loaded_removed_children = set()
         self._non_loaded_removed_forward_links = set()
         self._non_loaded_removed_reverse_links = SetMultimap()
+        self.__object_id = self._backing_record.record_id
 
     def __hash__(self):
-        return self._backing_record.__hash__()
+        return self.__object_id.__hash__()
 
     def __eq__(self, other):
         if not isinstance(other, PyRecordModel):
             return False
         return self._backing_record.__eq__(other._backing_record)
 
     @property
@@ -433,14 +437,15 @@
             self.set_field_value(field_name, link_to.record_id)
 
     def delete(self) -> None:
         """
         Flag the current record model to be deleted on commit.
         """
         from sapiopylib.rest.utils.recordmodel.RecordModelEvents import RecordDeletedEvent
+        self.__is_deleted = True
         self._record_model_manager.event_bus.fire_record_delete_event(RecordDeletedEvent(self))
 
     def _set_field_direct(self, field_name: str, field_value: Any) -> None:
         """
         Set field directly without firing an event or perform equality check. This is an internal method.
         """
         # noinspection PyProtectedMember
@@ -573,7 +578,8 @@
             return
         self._backing_record.set_fields(self.fields.copy_to_dict())
         self._backing_record.commit_changes()
 
     @property
     def record_model_manager(self):
         return self._record_model_manager
+
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,18 +152,15 @@
     def _on_commit(self):
         all_recs = set(self.__record_by_record_id.values())
         for record in all_recs:
             record.do_commit()
             # Update for records with negative Record ID with a new reference point.
             if record.record_id not in self.__record_by_record_id:
                 self.__record_by_record_id[record.record_id] = record
-        # Remove all negative record ID references we have now
-        negative_record_ids = [x for x in self.__record_by_record_id.keys() if x < 0]
-        for record_id in negative_record_ids:
-            del self.__record_by_record_id[record_id]
+        # DO NOT Remove all negative record ID references we have now, for side link cache references.
 
     @property
     def record_model_manager(self):
         return self._record_model_manager
 
     @property
     def event_bus(self):
```

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.8.8.149/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/LICENSE` & `sapiopylib-2023.8.8.149/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/README.md` & `sapiopylib-2023.8.8.149/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.8.142/pyproject.toml` & `sapiopylib-2023.8.8.149/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.06.08.142'
+version='2023.08.08.149'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -21,15 +21,15 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    'Development Status :: 4 - Beta',
+    'Development Status :: 5 - Production/Stable',
 ]
 homepage = "https://www.sapiosciences.com/"
 keywords = ["lims", "eln", "rest", "sapio"]
 
 [project.urls]
 "Homepage" = "https://github.com/sapiosciences"
 "Bug Tracker" = "https://github.com/sapiosciences/sapio-py-tutorials/issues"
```

### Comparing `sapiopylib-2023.6.8.142/PKG-INFO` & `sapiopylib-2023.8.8.149/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.6.8.142
+Version: 2023.8.8.149
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

