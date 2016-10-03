# deprecated-dojo

Let's build a complete list of dojo deprecated api, to support [anti-babel](https://github.com/gratex/anti-babel), git-qa and other code quality and refactoring tools.

## TL;DR Results
	
This all seems to be somehow deprecated, by release notes, reference guide or by api docs:

	./bin/deprecated 

Note list has some false positives (example dojo/has reference guide column), 
I will filter them later by manual inspection (probably).


|mid|rel-notes|ref-guide|api-doc|
|-----|---------|---------|---|
|dijit/Calendar|-|-|4|
|dijit/Calendar.\_MonthDropDown|-|-|3|
|dijit/Calendar.\_MonthDropDownButton|-|-|8|
|dijit/CheckedMenuItem|-|-|5|
|dijit/ColorPalette|-|-|3|
|dijit/ConfirmDialog|-|-|8|
|dijit/ConfirmTooltipDialog|-|-|8|
|dijit/Declaration|-|-|3|
|dijit/Dialog|-|-|8|
|dijit/Dialog.\_DialogBase|-|-|2|
|dijit/DialogUnderlay|-|-|3|
|dijit/DropDownMenu|-|-|5|
|dijit/Editor|-|-|6|
|dijit/Fieldset|-|-|7|
|dijit/InlineEditBox|-|-|6|
|dijit/InlineEditBox.\_InlineEditor|-|-|3|
|dijit/Menu|-|-|5|
|dijit/MenuBar|-|-|5|
|dijit/MenuBarItem|-|-|5|
|dijit/MenuItem|-|-|5|
|dijit/PopupMenuBarItem|-|-|5|
|dijit/PopupMenuItem|-|-|5|
|dijit/ProgressBar|-|-|3|
|dijit/RadioMenuItem|-|-|5|
|dijit/TitlePane|-|-|7|
|dijit/Toolbar|-|-|5|
|dijit/ToolbarSeparator|-|-|3|
|dijit/Tooltip|-|-|3|
|dijit/Tooltip.\_MasterTooltip|-|-|3|
|dijit/TooltipDialog|-|-|8|
|dijit/Tree|-|-|6|
|dijit/Tree.\_TreeNode|-|-|4|
|dijit/\_BidiSupport|-|2|-|
|dijit/\_Container|-|-|1|
|dijit/\_KeyNavContainer|-|-|2|
|dijit/\_MenuBase|-|-|5|
|dijit/\_Templated|-|-|1|
|dijit/\_TimePicker|-|-|1|
|dijit/\_Widget|-|-|3|
|dijit/\_editor/RichText|-|-|6|
|dijit/\_editor/plugins/FontChoice.\_FontDropDown|-|-|3|
|dijit/\_editor/plugins/FontChoice.\_FontNameDropDown|-|-|3|
|dijit/\_editor/plugins/FontChoice.\_FontSizeDropDown|-|-|4|
|dijit/\_editor/plugins/FontChoice.\_FormatBlockDropDown|-|-|3|
|dijit/form/Button|-|-|7|
|dijit/form/CheckBox|-|-|8|
|dijit/form/ComboBox|-|-|9|
|dijit/form/ComboButton|-|-|8|
|dijit/form/CurrencyTextBox|-|-|9|
|dijit/form/DateTextBox|-|-|9|
|dijit/form/DropDownButton|-|-|8|
|dijit/form/FilteringSelect|-|-|9|
|dijit/form/Form|-|-|5|
|dijit/form/HorizontalRule|-|-|3|
|dijit/form/HorizontalRuleLabels|-|-|3|
|dijit/form/HorizontalSlider|-|-|7|
|dijit/form/MappedTextBox|-|-|9|
|dijit/form/MultiSelect|-|-|6|
|dijit/form/NumberSpinner|-|-|9|
|dijit/form/NumberTextBox|-|-|9|
|dijit/form/RadioButton|-|-|8|
|dijit/form/RangeBoundTextBox|-|-|9|
|dijit/form/Select|-|-|7|
|dijit/form/Select.\_Menu|-|-|5|
|dijit/form/SimpleTextarea|-|-|8|
|dijit/form/Slider|-|3|-|
|dijit/form/TextBox|-|-|8|
|dijit/form/Textarea|-|-|8|
|dijit/form/TimeTextBox|-|-|9|
|dijit/form/ToggleButton|-|-|8|
|dijit/form/ValidationTextBox|-|-|9|
|dijit/form/VerticalRule|-|-|3|
|dijit/form/VerticalRuleLabels|-|-|3|
|dijit/form/VerticalSlider|-|-|7|
|dijit/form/\_DateTimeTextBox|-|-|9|
|dijit/form/\_FormMixin|-|-|2|
|dijit/form/\_FormSelectWidget|-|-|7|
|dijit/form/\_FormValueWidget|-|-|6|
|dijit/form/\_FormWidget|-|-|6|
|dijit/form/\_Spinner|-|-|9|
|dijit/index|-|4|-|
|dijit/layout/AccordionContainer|-|-|4|
|dijit/layout/AccordionContainer.\_Button|-|-|3|
|dijit/layout/AccordionContainer.\_InnerContainer|-|-|3|
|dijit/layout/AccordionPane|-|-|7|
|dijit/layout/BorderContainer|-|-|4|
|dijit/layout/BorderContainer.\_Gutter|-|-|3|
|dijit/layout/BorderContainer.\_Splitter|-|-|3|
|dijit/layout/ContentPane|-|-|6|
|dijit/layout/LayoutContainer|-|-|4|
|dijit/layout/LinkPane|-|-|6|
|dijit/layout/ScrollingTabController|-|-|4|
|dijit/layout/SplitContainer|-|-|5|
|dijit/layout/StackContainer|-|-|4|
|dijit/layout/StackController|-|-|4|
|dijit/layout/StackController.StackButton|-|-|8|
|dijit/layout/TabContainer|-|-|4|
|dijit/layout/TabController|-|-|4|
|dijit/layout/TabController.TabButton|-|-|8|
|dijit/layout/\_LayoutWidget|-|-|4|
|dijit/layout/\_TabContainerBase|-|-|4|
|dijit/main.\_Calendar|-|-|4|
|dijit/main.place|-|-|1|
|dijit/place|-|-|1|
|dijit/tree/Model|-|3|-|
|dojo/NodeList|-|1|-|
|dojo/NodeList-dom|-|4|-|
|dojo/\_base/config|-|4|-|
|dojo/\_base/connect|-|3|1|
|dojo/\_base/declare|-|3|-|
|dojo/\_base/event|-|3|-|
|dojo/\_base/index|-|4|-|
|dojo/\_base/json|-|3|-|
|dojo/\_base/kernel|-|3|4|
|dojo/\_base/lang|-|3|-|
|dojo/\_base/loader|-|4|-|
|dojo/addOnLoad|-|4|-|
|dojo/base/loader|-|1|-|
|dojo/coords|-|5|-|
|dojo/data/ItemFileReadStore|-|-|3|
|dojo/data/ItemFileWriteStore|-|-|3|
|dojo/declare|-|2|-|
|dojo/deprecated|-|5|-|
|dojo/dnd|-|3|-|
|dojo/dom|-|3|-|
|dojo/dom-attr|-|3|-|
|dojo/dom-class|-|3|-|
|dojo/dom-construct|-|3|-|
|dojo/dom-form|-|3|-|
|dojo/dom-geometry|-|3|-|
|dojo/dom-prop|-|3|-|
|dojo/gears|-|3|-|
|dojo/has|-|3|-|
|dojo/index|-|5|-|
|dojo/main|-|-|4|
|dojo/moduleUrl|-|1|-|
|dojo/parser|-|3|-|
|dojo/position|-|2|-|
|dojo/registerModulePath|-|1|-|
|dojo/store/JsonRest|-|3|-|
|dojox/app|-|3|-|
|dojox/app/widgets/Container|-|-|1|
|dojox/atom/widget/FeedEntryEditor|-|-|4|
|dojox/atom/widget/FeedEntryViewer|-|-|4|
|dojox/atom/widget/FeedEntryViewer.EntryHeader|-|-|4|
|dojox/atom/widget/FeedViewer|-|-|4|
|dojox/atom/widget/FeedViewer.FeedViewerEntry|-|-|3|
|dojox/atom/widget/FeedViewer.FeedViewerGrouping|-|-|3|
|dojox/av/FLVideo|-|-|3|
|dojox/av/widget/PlayButton|-|-|3|
|dojox/av/widget/Player|-|-|3|
|dojox/av/widget/ProgressSlider|-|-|3|
|dojox/av/widget/Status|-|-|3|
|dojox/av/widget/VolumeButton|-|-|3|
|dojox/charting|-|3|-|
|dojox/charting/action2d/\_IndicatorElement|-|-|1|
|dojox/charting/plot2d/Areas|-|-|1|
|dojox/charting/plot2d/Bars|-|-|1|
|dojox/charting/plot2d/Base|-|-|1|
|dojox/charting/plot2d/Bubble|-|-|1|
|dojox/charting/plot2d/Candlesticks|-|-|1|
|dojox/charting/plot2d/CartesianBase|-|-|1|
|dojox/charting/plot2d/ClusteredBars|-|-|1|
|dojox/charting/plot2d/ClusteredColumns|-|-|1|
|dojox/charting/plot2d/Columns|-|-|1|
|dojox/charting/plot2d/Default|-|-|1|
|dojox/charting/plot2d/Grid|-|-|1|
|dojox/charting/plot2d/Indicator|-|-|1|
|dojox/charting/plot2d/Lines|-|-|1|
|dojox/charting/plot2d/Markers|-|-|1|
|dojox/charting/plot2d/MarkersOnly|-|-|1|
|dojox/charting/plot2d/OHLC|-|-|1|
|dojox/charting/plot2d/Pie|-|-|1|
|dojox/charting/plot2d/Scatter|-|-|1|
|dojox/charting/plot2d/Spider|-|-|1|
|dojox/charting/plot2d/Stacked|-|-|1|
|dojox/charting/plot2d/StackedAreas|-|-|1|
|dojox/charting/plot2d/StackedBars|-|-|1|
|dojox/charting/plot2d/StackedColumns|-|-|1|
|dojox/charting/plot2d/StackedLines|-|-|1|
|dojox/data|Deprecated|-|-|
|dojox/data/AndOrReadStore|Deprecated|-|3|
|dojox/data/AndOrWriteStore|Deprecated|-|3|
|dojox/data/AppStore|Deprecated|-|-|
|dojox/data/AtomReadStore|Deprecated|-|-|
|dojox/data/ClientFilter|Deprecated|-|-|
|dojox/data/CouchDBRestStore|Deprecated|-|-|
|dojox/data/CssClassStore|Deprecated|-|-|
|dojox/data/CssRuleStore|Deprecated|-|-|
|dojox/data/CsvStore|Deprecated|-|-|
|dojox/data/FileStore|Deprecated|-|-|
|dojox/data/FlickrRestStore|Deprecated|-|-|
|dojox/data/FlickrStore|Deprecated|-|-|
|dojox/data/GoogleFeedStore|Deprecated|-|-|
|dojox/data/GoogleSearchStore|Deprecated|-|-|
|dojox/data/HtmlStore|Deprecated|-|-|
|dojox/data/HtmlTableStore|Deprecated|5|1|
|dojox/data/JsonRestStore|Deprecated|-|-|
|dojox/data/KeyValueStore|Deprecated|-|-|
|dojox/data/OpenSearchStore|Deprecated|-|-|
|dojox/data/OpmlStore|Deprecated|-|-|
|dojox/data/PersevereStore|Deprecated|-|-|
|dojox/data/PicasaStore|Deprecated|-|-|
|dojox/data/QueryReadStore|Deprecated|-|-|
|dojox/data/RailsStore|Deprecated|-|-|
|dojox/data/S3Store|Deprecated|-|-|
|dojox/data/ServiceStore|Deprecated|-|-|
|dojox/data/WikipediaStore|Deprecated|-|-|
|dojox/data/XmlStore|Deprecated|-|-|
|dojox/data/dom|-|-|1|
|dojox/drawing/plugins/drawing/GreekPalette|-|-|3|
|dojox/dtl/contrib/dom|-|-|1|
|dojox/editor/plugins|Various|-|-|
|dojox/editor/plugins/AutoSave.\_AutoSaveSettingDialog|-|-|3|
|dojox/editor/plugins/Breadcrumb.\_BreadcrumbMenuTitle|-|-|3|
|dojox/editor/plugins/CollapsibleToolbar.\_CollapsibleToolbarButton|-|-|3|
|dojox/editor/plugins/EntityPalette|-|-|3|
|dojox/editor/plugins/FindReplace.\_FindReplaceCheckBox|-|-|3|
|dojox/editor/plugins/FindReplace.\_FindReplaceCloseBox|-|-|3|
|dojox/editor/plugins/FindReplace.\_FindReplaceTextBox|-|-|3|
|dojox/editor/plugins/FindReplace.\_FindReplaceToolbar|-|-|5|
|dojox/editor/plugins/SpellCheck.\_SpellCheckControl|-|-|3|
|dojox/editor/plugins/StatusBar.\_StatusBar|-|-|3|
|dojox/editor/plugins/TextColor.\_TextColorDropDown|-|-|3|
|dojox/editor/plugins/ToolbarLineBreak|-|-|3|
|dojox/editor/plugins/\_SmileyPalette|-|-|3|
|dojox/embed/Object|-|-|3|
|dojox/form/BusyButton|-|-|7|
|dojox/form/CheckedMultiSelect|-|-|7|
|dojox/form/DateTextBox|-|-|9|
|dojox/form/DayTextBox|-|-|9|
|dojox/form/DropDownSelect|Deprecated|5|7|
|dojox/form/DropDownSelect.\_Menu|-|-|5|
|dojox/form/FileInput|-|-|6|
|dojox/form/FileInputAuto|-|-|6|
|dojox/form/FileInputBlind|-|-|6|
|dojox/form/FilePickerTextBox|-|-|9|
|dojox/form/FileUploader|Deprecated|4|3|
|dojox/form/HorizontalRangeSlider|-|-|7|
|dojox/form/ListInput|-|-|6|
|dojox/form/Manager|-|-|3|
|dojox/form/MonthTextBox|-|-|9|
|dojox/form/MultiComboBox|-|-|9|
|dojox/form/PasswordValidator|-|-|6|
|dojox/form/Rating|-|-|5|
|dojox/form/TimeSpinner|-|-|9|
|dojox/form/TriStateCheckBox|-|-|8|
|dojox/form/Uploader|-|-|7|
|dojox/form/VerticalRangeSlider|-|-|7|
|dojox/form/YearTextBox|-|-|9|
|dojox/form/\_FormSelectWidget|-|-|7|
|dojox/form/uploader/FileList|-|-|3|
|dojox/form/uploader/\_Base|-|-|3|
|dojox/fx|-|1|-|
|dojox/fx/Shadow|-|-|3|
|dojox/fx/easing|Deprecated|-|-|
|dojox/gauges|Deprecated|-|-|
|dojox/gauges/AnalogArcIndicator|-|-|3|
|dojox/gauges/AnalogArrowIndicator|-|-|3|
|dojox/gauges/AnalogCircleIndicator|-|-|3|
|dojox/gauges/AnalogGauge|-|-|3|
|dojox/gauges/AnalogIndicatorBase|-|-|3|
|dojox/gauges/AnalogLineIndicator|-|-|3|
|dojox/gauges/AnalogNeedleIndicator|-|-|3|
|dojox/gauges/BarCircleIndicator|-|-|3|
|dojox/gauges/BarGauge|-|-|3|
|dojox/gauges/BarIndicator|-|-|3|
|dojox/gauges/BarLineIndicator|-|-|3|
|dojox/gauges/GlossyCircularGauge|-|-|3|
|dojox/gauges/GlossyCircularGaugeBase|-|-|3|
|dojox/gauges/GlossyCircularGaugeNeedle|-|-|3|
|dojox/gauges/GlossyHorizontalGauge|-|-|3|
|dojox/gauges/GlossyHorizontalGaugeMarker|-|-|3|
|dojox/gauges/GlossySemiCircularGauge|-|-|3|
|dojox/gauges/Range|-|-|3|
|dojox/gauges/TextIndicator|-|-|3|
|dojox/gauges/\_Gauge|-|-|3|
|dojox/gauges/\_Indicator|-|-|3|
|dojox/geo/charting/widget/Legend|-|-|3|
|dojox/geo/charting/widget/Map|-|-|3|
|dojox/geo/openlayers/widget/Map|-|-|3|
|dojox/gfx|-|2|-|
|dojox/grid|Deprecated|-|-|
|dojox/grid/DataGrid|-|-|6|
|dojox/grid/EnhancedGrid|-|-|6|
|dojox/grid/LazyTreeGrid|-|-|6|
|dojox/grid/TreeGrid|-|-|6|
|dojox/grid/\_Grid|-|-|6|
|dojox/grid/\_RowSelector|-|-|3|
|dojox/grid/\_Selector|-|-|3|
|dojox/grid/\_TreeView|-|-|3|
|dojox/grid/\_View|-|-|3|
|dojox/grid/cells/dijit.CheckBox|-|-|1|
|dojox/grid/cells/dijit.ComboBox|-|-|1|
|dojox/grid/cells/dijit.DateTextBox|-|-|1|
|dojox/grid/cells/dijit.Editor|-|-|1|
|dojox/grid/cells/dijit.\_Widget|-|-|1|
|dojox/grid/enhanced/plugins/Dialog|-|-|8|
|dojox/grid/enhanced/plugins/Pagination|-|-|4|
|dojox/grid/enhanced/plugins/filter/ClearFilterConfirm|-|-|3|
|dojox/grid/enhanced/plugins/filter/FilterBar|-|-|3|
|dojox/grid/index|-|5|-|
|dojox/help|Abandoned|-|-|
|dojox/highlight/widget/Code|-|-|3|
|dojox/image/Badge|-|-|3|
|dojox/image/Gallery|Abandoned|-|-|
|dojox/image/Magnifier|-|-|3|
|dojox/image/MagnifierLite|-|-|3|
|dojox/image/SlideShow|Abandoned|-|-|
|dojox/image/TumbnailPicker|Abandoned|-|-|
|dojox/index|-|5|-|
|dojox/info|-|5|-|
|dojox/io/scriptFrame|Deprecated|-|-|
|dojox/io/windowName|Deprecated|-|-|
|dojox/io/xhrMultiPart|Deprecated|-|-|
|dojox/io/xhrPlugins|Deprecated|-|-|
|dojox/lang/observable|Deprecated|-|-|
|dojox/layout/ContentPane|-|-|6|
|dojox/layout/DragPane|-|-|3|
|dojox/layout/ExpandoPane|-|-|6|
|dojox/layout/FloatingPane|-|-|7|
|dojox/layout/GridContainer|-|-|4|
|dojox/layout/GridContainerLite|-|-|4|
|dojox/layout/ResizeHandle|-|-|3|
|dojox/layout/RotatorContainer|-|5|4|
|dojox/layout/ScrollPane|-|-|6|
|dojox/layout/TableContainer|-|-|4|
|dojox/mobile/Accordion|-|-|1|
|dojox/mobile/Carousel|-|-|1|
|dojox/mobile/Container|-|-|1|
|dojox/mobile/ContentPane|-|-|1|
|dojox/mobile/DataCarousel|-|-|1|
|dojox/mobile/EdgeToEdgeDataList|-|-|1|
|dojox/mobile/EdgeToEdgeList|-|-|1|
|dojox/mobile/EdgeToEdgeStoreList|-|-|1|
|dojox/mobile/FixedSplitter|-|-|1|
|dojox/mobile/FixedSplitterPane|-|1|1|
|dojox/mobile/FormLayout|-|-|1|
|dojox/mobile/GridLayout|-|-|1|
|dojox/mobile/Heading|-|-|1|
|dojox/mobile/IconContainer|-|-|1|
|dojox/mobile/IconItem|-|-|1|
|dojox/mobile/IconMenu|-|-|1|
|dojox/mobile/IconMenuItem|-|-|1|
|dojox/mobile/ListItem|-|2|1|
|dojox/mobile/RoundRect|-|-|1|
|dojox/mobile/RoundRectDataList|-|-|1|
|dojox/mobile/RoundRectList|-|-|1|
|dojox/mobile/RoundRectStoreList|-|-|1|
|dojox/mobile/ScrollableView|-|-|1|
|dojox/mobile/SpinWheel|-|-|1|
|dojox/mobile/SpinWheelDatePicker|-|-|1|
|dojox/mobile/SpinWheelTimePicker|-|-|1|
|dojox/mobile/StoreCarousel|-|-|1|
|dojox/mobile/SwapView|-|-|1|
|dojox/mobile/TabBar|-|-|1|
|dojox/mobile/TabBarButton|-|-|1|
|dojox/mobile/ToolBarButton|-|-|1|
|dojox/mobile/TreeView|-|-|1|
|dojox/mobile/ValuePicker|-|-|1|
|dojox/mobile/ValuePickerDatePicker|-|-|1|
|dojox/mobile/ValuePickerTimePicker|-|-|1|
|dojox/mobile/View|-|-|1|
|dojox/mobile/\_ItemBase|-|-|1|
|dojox/mobile/\_PickerBase|-|-|1|
|dojox/mobile/app|Deprecated|-|-|
|dojox/mobile/differences-17-18|-|3|-|
|dojox/mobile/internationalization|-|2|-|
|dojox/mvc|-|3|-|
|dojox/mvc/Bind.WidgetList|-|-|1|
|dojox/mvc/WidgetList|-|-|1|
|dojox/mvc/\_base.WidgetList|-|-|1|
|dojox/presentation|-|5|-|
|dojox/rpc/smd|-|3|-|
|dojox/secure|Abandoned|-|-|
|dojox/sketch/Toolbar|-|-|5|
|dojox/sql|Abandoned|-|-|
|dojox/storage|Abandoned|-|-|
|dojox/widget/AnalogGauge|Abandoned|-|-|
|dojox/widget/BarGauge|Abandoned|-|-|
|dojox/widget/Calendar|-|-|1|
|dojox/widget/Calendar2Pane|-|-|1|
|dojox/widget/Calendar3Pane|-|-|1|
|dojox/widget/CalendarFisheye|-|-|1|
|dojox/widget/CalendarFx|-|-|1|
|dojox/widget/ColorPicker|-|-|6|
|dojox/widget/DailyCalendar|-|-|1|
|dojox/widget/DataPresentation|Abandoned|-|-|
|dojox/widget/DialogSimple|-|-|8|
|dojox/widget/DocTester|Abandoned|-|-|
|dojox/widget/DynamicTooltip|Abandoned|-|-|
|dojox/widget/FilePicker|Abandoned|-|-|
|dojox/widget/FisheyeList|-|-|1|
|dojox/widget/Iterator|Abandoned|-|-|
|dojox/widget/Loader|Abandoned|-|-|
|dojox/widget/MonthAndYearlyCalendar|-|-|1|
|dojox/widget/MonthlyCalendar|-|-|1|
|dojox/widget/MultiSelectCalendar|-|-|3|
|dojox/widget/MultiSelectCalendar.\_MonthDropDown|-|-|3|
|dojox/widget/PlaceholderMenuItem|-|-|5|
|dojox/widget/Portlet|-|-|7|
|dojox/widget/PortletDialogSettings|-|-|6|
|dojox/widget/PortletSettings|-|-|6|
|dojox/widget/RollingList|Abandoned|-|-|
|dojox/widget/Rotator|Abandoned|-|-|
|dojox/widget/SortList|Abandoned|-|-|
|dojox/widget/Standby|-|-|3|
|dojox/widget/TitleGroup|-|-|3|
|dojox/widget/Wizard|-|-|4|
|dojox/widget/WizardPane|-|-|6|
|dojox/widget/YearlyCalendar|-|-|1|
|dojox/widget/\_CalendarBase|-|-|1|
|dojox/wire|Abandoned|-|-|
|dojox/wire/ml|Abandoned|-|-|
|dojox/xmpp|Abandoned|-|-|
|util/doctools/markup|-|2|-|
|util/index|-|3|-|


## Problem

dojo is not very consistent in marking the codes as deprecated, 
this may help you (helped us)

Examples of inconsistencies:

dojo/_base/lang methods 
- not marked in source code
- not marked in api docs (detail.json)
- marked in reference guide

Another problem is that some methods you will never find in documentation:

Example, dojo functional and unzip

	< ../dojo-website/src/documentation/api/1.10/details.json grep unzip

## Install and try
	
	# get tools
	npm install

	# not using submodule, gh-pages problem
	# get/update dojo data (api and reference guide)
	# git submodule init
	# git submodule update

	# do
	git clone -b master --single-branch https://github.com/dojo/dojo-website.git

	# or if clone somewhere on disk adjust paths

	# methods deprecated in API docs (detail.json)
	./bin/deprecated-api dojo-website/src/documentation/api/1.10/details.json

	# modules with some deprecated apis
	./bin/deprecated-reference-guide

Samples:

	./bin/deprecated-api dojo-website/src/documentation/api/1.10/details.json | wc -l
	    1163
	 ./bin/deprecated-api dojo-website/src/documentation/api/1.9/details.json | wc -l
	    1128
	./bin/deprecated-api dojo-website/src/documentation/api/1.8/details.json | wc -l
	     972	

## For review

Intersection of our used modules with deprecated APIs:

	git grep -h -w -f ./doc/used-modules.txt deprecated.md


