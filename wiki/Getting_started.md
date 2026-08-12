# Getting started
## Foreword

ဖရီးကက် (FreeCAD) သည် 3D [parametric modeling application](About_FreeCAD.md) တစ်ခုဖြစ်သည်။ ဤအရာကို အဓိကအားဖြင့် မက်ကန်းနစ်ဒီဇိုင်းအတွက် ဖန်တီးထားသော်လည်း 3D ပစ္စည်းများကို တိကျမှုနှင့် မော်ဒယ်လုပ်ဆုံသက်မှတ်မှုကို ထိန်းချုပ်ကာ မော်ဒယ်တည်ဆောက်ရန် လိုအပ်သည့် အခြားအရာများတွင်လည်း အသုံးပြုနိုင်သည်။

ဖရီးကက် (FreeCAD) ကို 2002 ခုနှစ်တွင် ဖွံ့ဖြိုးရေးစတင်ခဲ့ပြီး [features](Feature_list.md) အများကြီးပါရှိသည်။ အချို့သောစွမ်းဆောင်ရည်များ မပြည့်စုံသေးပေမယ့် Hobbyist များနှင့် သေးငယ်သောလုပ်ငန်းခန်းများအတွက် လုံလောက်စွာ အင်အားရှိပြီဖြစ်သည်။ ဖရီးကက် (FreeCAD) အသုံးပြုသူများ၏ စိတ်အားထက်သန်မှုမြင့် သ [+community+] 는 ဖွံ့ဖြိုးလျက်ရှိပြီး [FreeCAD forum](http://forum.freecad.org/index.php) တွင် ပါဝင်ဆွေးနွေးကြသည်။ ဤဖိုရမ်တွင် ဖရီးကက် (FreeCAD) ဖြင့် ဖန်တီးထားသော အရည်အသွေးမြင့် project များ၏ [ဥပမာများ](https://forum.freecad.org/viewforum.php?f=24) အများရှိသည်။

အခမဲ့ဆော့ဖ်ဝဲပရောဂျက်များနှင့်တူ၊ ဖရီးကက် (FreeCAD) သည် မကြာခဏ ကြီးထွားလာရန်၊ လက်ရှေ့ပစ္စည်းများ ထည့်သွင်းရန်နှင့် bug များကို ပြန်လည်ပြင်ဆင်ရန် အသုံးပြုသူ အသိုင်းအဝိုင်းပေါ် မူတည်သည်။ ဖရီးကက် (FreeCAD) ကို အသုံးပြုသည့်အခါ ဤအချက်ကို မမေ့ပါနဲ့။ သင် ကြိုက်နှစ်သက်ပါက [donate](Donate.md) ပြုလုပ်နိုင်ပြီးစာရွက်စာတမ်းရေးခြင်း၊ ဘာသာပြန်ခြင်းစသဖြင့် အမျိုးမျိုးသောနည်းလမ်းများဖြင့် [help FreeCAD](Help_FreeCAD.md) ပြုနိုင်သည်။

ပြန်လည်ကြည့်ရန်။

-   [Migrating to FreeCAD from Fusion360](Migrating_to_FreeCAD_from_Fusion360.md)
-   [Which workbench should I choose?](Which_workbench_should_I_choose.md)
-   [Tutorials](Tutorials.md)
-   [Video tutorials](Video_tutorials.md)

## Installing

ပထမဦးဆုံး ဖရီးကက် (FreeCAD) ကို ဒေါင်းလုတ်၍ ထည့်သွင်းပါ။ ပစ္စည်းဗားရှင်းများနှင့် အပ်ဒိတ်များဆိုင်ရာ အချက်အလက်များအတွက် [Download](Download.md) စာမျက်နှာကို ကြည့်ပါ၊ သင့် OS အတွက် ထည့်သွင်းပုံညွှန်ကြားချက်များကိုလည်း ကြည့်ပါ ([Windows](Installing_on_Windows.md), [Linux](Installing_on_Linux.md) သို့မဟုတ် [macOS](Installing_on_Mac.md))။ Linux ဖြန့်ဖြူးမှုများ၏ package manager များမှလည်း ဖရီးကက် (FreeCAD) ကို ရရှိနိုင်သည်။ ဖရီးကက် (FreeCAD) သည် open-source ဖြစ်လို့ source code ကိုလည်း ဆွဲယူကာ ကိုယ့်အဖွဲ့လိုက် [compile](Compiling.md) လုပ်နိုင်ပါသည်။

## Exploring the interface 

<img alt="" src=images/FreeCAD_interface_base_divisions.svg  style="width:1024px;">



*The standard FreeCAD interface*


**See a full explanation in [Interface](Interface.md).**


:   1\. The [main view area](main_view_area.md), which can contain different tabbed windows, principally the [3D view](3D_view.md).
:   2\. The [3D view](3D_view.md), showing the geometrical objects in the document.
:   3\. The [tree view](tree_view.md) (part of the [combo view](combo_view.md)), showing the hierarchy and construction history of objects in the document; it can also display the [task panel](task_panel.md) for active commands.
:   4\. The [property editor](property_editor.md) (part of the [combo view](combo_view.md)), which allows viewing and modifying properties of the selected objects.
:   5\. The [selection view](selection_view.md), which indicates the objects or sub-elements of objects (vertices, edges, faces) that are selected.
:   6\. The [report view](report_view.md) (or output window), where messages, warnings and errors are shown.
:   7\. The [Python console](Python_console.md), where all the commands executed are printed, and where you can enter [Python](Python.md) code.
:   8\. The [status bar](status_bar.md), where some messages and tooltips appear.
:   9\. The toolbar area, where the toolbars are docked.
:   10\. The [workbench selector](Std_Workbench.md), where you select the active [workbench](workbenches.md).
:   11\. The [standard menu](Standard_Menu.md), which holds basic operations of the program.

FreeCAD ရဲ့ အင်တာဖေ့စ်၏ အဓိက အမြင်ကတော့ ၎င်းကို [workbenches](workbenches.md) အလိုက် ခွဲဝေထားခြင်း ဖြစ်သည်။ workbench ဆိုသည်မှာ တစ်စုံတစ်ရာ တာဝန်အတွက် သင့်တော်သည့် ကိရိယာများစုစည်းမှုတစ်ခု ဖြစ်ပြီး ဥပမာအားဖြင့် [meshes](Mesh_Workbench.md) များနှင့် အလုပ်လုပ်ရန် ၊ [2D objects](Draft_Workbench.md) ဆွဲရန် သို့မဟုတ် [ချိတ်ဆက်ထားသော စကစ်များ](Sketcher_Workbench.md) အတွက် အသုံးပြုနိုင်သော ကိရိယာများ ဖြစ်သည်။ လက်ရှိ workbench ကို [workbench selector](Std_Workbench.md) မှတစ်ဆင့် ပြောင်းလဲနိုင်သည်။ သင်သည် workbench တစ်ခုစီတွင် ပါရှိသည့် ကိရိယာများကို [customize](Interface_Customization.md) လုပ်၍ အခြား workbench များမှ ကိရိယာများ ထည့်စရာပေးနိုင်သည်၊ သင်ကိုယ်တိုင် ဖန်တီးထားသော ကိရိယာများ (យើងက [macros](macros.md) ဟု ခေါ်တတ်သည်) ကိုပါ ထည့်နိုင်သည်။ များစွာ အသုံးပြုသော စတင်နေရာများမှာ [PartDesign Workbench](PartDesign_Workbench.md) နှင့် [Part Workbench](Part_Workbench.md) တို့ ဖြစ်သည်။

FreeCAD ကို ပထမဆုံး စတင်ချိန်တွင် Start စာမျက်နှာကို မျှင်ကြည့်ရမည်။ ဗားရှင်း 0.19 အတွက် Start စာမျက်နှာကို အောက်က ကဲ့သို့ တွေ့ရသည်။

<img alt="" src=images/Start_center_0.19_screenshot.png  style="width:600px;">

Start စာမျက်နှာမှ စတင်၍ အများအားဖြင့် သုံးသော workbench တစ်ခုသို့ အမြန်ကူးနိုင်သည်၊ သြဇာဖိုင်များထဲမှ သစ်ပင်(Recent files) တစ်ခုဖွင့်နိုင်သည်၊ သို့မဟုတ် ဖရီးကက် (FreeCAD) သတင်းများကို ကြည့်ရှုနိုင်သည်။ ပဒီဖောထည့်ထားသော workbench ကို [preferences](Preferences_Editor.md) တွင် ပြောင်းလဲနိုင်သည်။

## Navigating in the 3D space 

ဖရီးကက် (FreeCAD) တွင် [navigation modes](Mouse_navigation.md) များစွာ ရရှိနိုင်ပြီး ၎င်းများသည် 3D view တွင် object များနှင့် ပြုလုပ်သည့် မောက်စ်အသုံးပြုမှုနည်းလမ်းကို ပြောင်းလဲပေးသည်။ ထို modes များအနက် တစ်ခုမှာ [touchpads](Mouse_navigation#Touchpad_navigation.md) များအတွက် ထူးခြားစွာ ပြုလုပ်ထားပြီး မကြိမ်မရောက် မော်တစ်ခုအလယ်ဘက်ခလုတ်အသုံးမပြုရပဲ အသုံးပြုနိုင်သည်။ ပဋိညာဉ်လိုက် navigation mode ပုံမှန်အားဖြင့် [CAD navigation](Mouse_navigation#CAD_navigation.md) ဖြစ်သည်။ လက်ရှိ navigation mode ကို အမြန်ပြောင်းရန် [Status bar](Status_bar.md) အတွင်းရှိ **[<img src=images/NavigationCAD_dark.svg style="width:16px">** ခလုတ်ကို အသုံးပြုနိုင်သည် သို့မဟုတ် [3D view](3D_view.md) ၏ ဗလာနေရာတစ်နေရာပေါ်တွင် right-click ပြုလုပ်၍လည်း ပြောင်းလဲနိုင်သည်။

View presets များ (top view၊ front view၊ စသည်) ကို View မီနူး၊ View toolbar နှင့် နံပါတ်ပေးထားသော ခလုတ်များ (**1**, **2**, စသဖြင့်) မှတစ်ဆင့်လည်း အသုံးပြုနိုင်သည်။ 3D view တွင် object တစ်ခုအား သို့မဟုတ် ဗလာနေရာတစ်ခုအား right-click ပြုလုပ်လျှင် ဗျည်းကို သတ်မှတ်ခြင်း၊ Tree view တွင် object ကို တည်နေရာပြခြင်းကဲ့သို့သော အသုံးများကို အမြန်ဝင်ရောက်နိုင်သည်။

## First steps with FreeCAD 

ဖရီးကက် (FreeCAD) ၏ အဓိက ရည်ရွယ်ချက်မှာ တိကျသော 3D မော်ဒယ်များကို ဖန်တီးရန်၊ ထိုမော်ဒယ်များအပေါ် တင်းကျပ်စွာ ထိန်းချုပ်နိုင်ရန် (မော်ဒယ်သမိုင်းသို့ ပြန်ဝင်ကာ ပမာဏများကို ပြောင်းနိုင်ရန်) နှင့် အခြားနောက်ဆုံးတွင် ထိုမော်ဒယ်များကို တည်ဆောက်နိုင်ရန် (3D printing, CNC machining သို့မဟုတ် ဆောက်လုပ်ရေးဝက်ဆိုက်ပေါ်တွင်) ဖြစ်သည်။ ထို့ကြောင့် ဤသည်မှာ အခြား 3D အက်ပလီကေးရှင်းများ (ကာတွန်းဇာတ်လမ်း သို့မဟုတ် ဂိမ်းများအတွက် ဖန်တီးထားသည့်) ထက် မတူကွာခြားသည်။ သင်အကယ်၍ 3D မော်ဒယ်လုပ်ခြင်းကို ပထမဆုံးကြုံတွေ့နေပါက သင်ယူရန် လမ်းကြောင်းမှာ ခက်ခဲနိုင်သည်။ မည်သည့်အချိန်တွင် မတက်နိုင်သလို အခက်အခဲရှိခဲ့လျှင် [FreeCAD forum](http://forum.freecad.org/index.php) တွင် ရှိသော သဘောထားကောင်းသော အသုံးပြုသူ အသိုင်းအဝိုင်းက သင့်ကို အမြန်ကူညီနိုင်သည်ကို မမေ့ပါနှင့်။

FreeCAD တွင် စတင်အသုံးပြုမည့် workbench ကို သင့်လုပ်ငန်းအမျိုးအစားပေါ် မူတည်သည်။ မက်ကန်းနစ် မော်ဒယ်များ သို့မဟုတ် အေသးစား ပစ္စည်းများပေါ် အလုပ်လုပ်မည်ဆိုလျှင် [PartDesign Workbench](PartDesign_Workbench.md) ကို စမ်းသပ်ချင်လိမ့်မည်။ 2D တွင် အလုပ်လုပ်မယ်ဆိုလျှင် [Draft Workbench](Draft_Workbench.md) သို့ ပြောင်းပါ၊ constraint များလိုအပ်ပါက [Sketcher Workbench](Sketcher_Workbench.md) သို့ ပြောင်းပါ။ BIM လုပ်ငန်းများအတွက် [BIM Workbench](BIM_Workbench.md) ကို ဖွင့်ပါ။ OpenSCAD ကမ္ဘာမှ လာသောသူများအတွက် [OpenSCAD Workbench](OpenSCAD_Workbench.md) ကိုစမ်းသပ်ပါ။ များသော အသိုင်းအဝိုင်းဖန်တီးထားသော [external workbenches](External_workbenches.md) များလည်း ရနိုင်ပါသည်။

Workbench များကို မည်သည့်အချိန်တွင်မဆို ပြောင်းလဲနိုင်ပြီး သင်နှစ်သက်သော workbench ကိုလည်း [customize](Interface_Customization.md) လုပ်၍ အခြား workbench များမှ ကိရိယာများ ထည့်နိုင်ပါသည်။

## Working with the PartDesign and Sketcher workbenches 

[PartDesign Workbench](PartDesign_Workbench.md) သည် ရှုပ်ထွေးသော ပစ္စည်းများကို တည်ဆောက်ရန် ဖန်တီးထားပြီး၊ ပုံမှန်အားဖြင့် ရိုးရှင်းသော ပုံစံများမှ စတင်ကာ အပိုင်းများ (အများအားဖြင့် "features" ဟု ခေါ်သည်) ကို ထည့်သွင်း သို့မဟုတ် ဖယ်ရှား၍ နောက်ဆုံး ပစ္စည်းကို ရောက်ရှိသည်။ မော်ဒယ်လုပ်စဉ်အတွင်း သင်အသုံးပြုသော feature အားလုံးကို [tree view](Document_structure.md) ဟု ခေါ်သော သီးခြားမြင်ကွင်းတွင် သိမ်းဆည်းထားသည်၊ ၎င်းတွင် စာရွက်စာတမ်းအတွင်းရှိ အခြား objects များလည်း ပါဝင်သည်။ PartDesign object ကို အစဉ်လိုက် လုပ်ဆောင်ချက်များ၏ ဆက်လက်တန်းလို ထင်မြင်နိုင်သည်။ တစ်ခုချင်းစီသည် ယခင်အရာ၏ ရလဒ်ပေါ်တွင်လက်ခံသတ်မှတ်ထားသော ကြိုးမဲ့တန်းဖြစ်သည်။ Tree view တွင် သင်၏ နောက်ဆုံးပစ္စည်းကို မြင်နိုင်သော်လည်း ၎င်းကို ဖွင့်၍ အရင်အခြေအနေများအားလုံးကို ပြန်လည်ရယူနိုင်ပြီး ၎င်းတို့၏ parameter များကို ပြောင်းလဲနိုင်သည်၊ ထို့နောက် နောက်ဆုံးပစ္စည်းသည် အလိုအလျောက် update လုပ်မည်။

PartDesign workbench သည် အခြား workbench တစ်ခုဖြစ်သော [Sketcher Workbench](Sketcher_Workbench.md) ကို အလေးထား အသုံးပြုသည်။ Sketcher သည် 2D ပုံစံများ ဆွဲရန် ခွင့်ပြုသည်၊ ဤ 2D ပုံစံများကို Constraint (ကန့်သတ်ချက်) များကို နှုတ်ဆက် အသုံးပြုကာ သတ်မှတ်သည်။ ဥပမာအားဖြင့် စတုရန်းတစ်ခု ဆွဲပြီး ထိုဘက်တစ်ဖက်၏ အရှည်ကို length ကန့်သတ်ချက်တစ်ခုဖြင့် သတ်မှတ်နိုင်သည်။ ထိုဘက်ကို ထပ်မံ ပြောင်းလဲ၍ မရတော့ပေ (ကန့်သတ်ချက်ကို ပြောင်းရန်မဟုတ်ရင်)။

Sketcher ဖြင့် ဖန်တီးထားသော 2D ပုံစံများကို PartDesign workbench တွင် အများအားဖြင့် အသုံးပြုသည်၊ ဥပမာ 3D အရွက်များ ဖန်တီးရန်၊ သို့မဟုတ် ပစ္စည်း၏ မျက်နှာများပေါ်တွင် ပုံစံများ ဆွဲ၍ ထိုနေရာများကို အဓိက အရွက်မှ ဖောက်ထုတ်ရန် စသည်ဖြင့် အသုံးပြုသည်။ ဤသည်မှာ PartDesign workflow တစ်ခု၏ နမူနာဖြစ်သည်။

1.  Create a new sketch
2.  Draw a closed shape (make sure all points are joined)
3.  Close the sketch
4.  Expand the sketch into a 3D solid by using the pad tool
5.  Select one face of the solid
6.  Create a second sketch (this time it will be drawn on the selected face)
7.  Draw a closed shape
8.  Close the sketch
9.  Create a pocket from the second sketch, on the first object

အထက်ဖော်ပြသည့် လုပ်ဆောင်မှုများကြောင့် အောက်ပါကဲ့သို့ အရာဝတ္ထုတစ်ခု ရရှိမည်။

 <img alt="" src=images/Partdesign_example.jpg  style="width:600px;"> 

မည်သည့်အချိန်တွင်မဆို မူလ sketch များကို ရွေးချယ်၍ ပြန်လည်ပြင်ဆင်နိုင်သည်၊ သို့မဟုတ် pad သို့ pocket လည်ပတ်မှုများ၏ extrusion parameter များကို အစားထိုးစစ်ဆေး ပြောင်းလဲနိုင်ပြီး ၎င်းသည် နောက်ဆုံးပစ္စည်းကို update လုပ်ပေးမည်။

## Working with the Draft and BIM workbenches 

[Draft Workbench](Draft_Workbench.md) နှင့် [BIM Workbench](BIM_Workbench.md) များသည် အခြား workbench များနှင့် မတူညီသော်လည်း FreeCAD အားလုံးတွင် သာမာန်ရှိသည့် စည်းမျဉ်းများကို ဖြတ်လျက် အလုပ်လုပ်ကြသည်။ ရိုးရိုးပြောရလျှင် Sketcher နှင့် PartDesign များသည် အထူးသဖြင့် တစ်ပစ္စည်းချင်းစီကို ဒီဇိုင်းလုပ်ရန် အဓိက ရည်ရွယ်ထားပေမယ့် Draft နှင့် BIM များသည် ပို၍ ရိုးရှင်းသည့် အစိတ်အပိုင်းများစွာနှင့် အလုပ်လုပ်သောအခါ သင့်အလုပ်ကို အလွယ်တကူ ပြုလုပ်နိုင်စေရန် ဖန်တီးထားသည်။

[Draft Workbench](Draft_Workbench.md) မှာ မူရင်း 2D CAD အက်ပလီကေးရှင်းများ (ဥပမာ [AutoCAD](https://en.wikipedia.org/wiki/AutoCAD)) တွင် တွေ့ရသလို 2D ကိရိယာများ အချို့ကို ပေးထားသည်။ သို့သော် Draft သည် FreeCAD ၏ အဓိက ရည်ရွယ်ချက်ဖြစ်သည့် 3D parametric modeling ထဲကနေ သိသိသာသာ ခွဲထွက်နေသောကြောင့် ထို 专门 applications များပေးသော ကိရိယာများစုံလင်မှုကို မမျှော်လင့်သင့်ပါ။ Draft ကိရိယာများ၏ တစ်ချို့ကို 2D မျက်နှာပြင်တွင်ပင်မဟုတ်ဘဲ အပြည့် 3D နေရာ၌လည်း အသုံးပြုနိုင်ပြီး [Work planes](Draft_SelectPlane.md) နှင့် [object snapping](Draft_Snap.md) ကဲ့သို့ အထူး အကူအညီစနစ်များအတွက် အကျိုးရှိသည်။

[BIM Workbench](BIM_Workbench.md) သည် FreeCAD ကို [BIM](http://en.wikipedia.org/wiki/Building_Information_Modeling) ကိရိယာများဖြင့် ဖျိုဖြည့်ပေးကာ parametric အဆောက်အအုံ မော်ဒယ်များ တည်ဆောက်နိုင်စေသည်။ BIM workbench သည် Draft နှင့် Sketcher ကဲ့သို့ အခြား module များကို ကျယ်ကျယ်ပြန့်ပြန့် အားပေးအသုံးပြုသည်။ Draft ကိရိယာများအားလုံးကို BIM workbench တွင်လည်း တွေ့နိုင်ပြီး BIM ကိရိယာအများစုသည် Draft ၏ helper systems များကို အသုံးပြုသည်။

BIM နှင့် Draft workbench များနှင့် သာမာန် workflow တစ်ခုဖြစ်နိုင်သည့် နမူနာကတော့ -

1.  Draft Line tool ဖြင့် လိုင်းများ တစ်နေရာချင်း ဆွဲပါ
2.  လိုင်းတိုင်းကို ရွေးချယ်ပြီး Wall tool ကိုနှိပ်၍ လိုင်းပေါ်တွင် နံရံတစ်ခု တည်ဆောက်ပါ
3.  နံရံများကို ရွေးချယ်ပြီး BIM Add tool ကို နှိပ်၍ ပေါင်းပါ
4.  Floor object တစ်ခု ဖန်တီး၍ Tree view တွင် သင့်နံရံများကို ထို floor object ထဲသို့ ဆွဲထည့်ပါ
5.  Building object တစ်ခု ဖန်တီးပြီး Tree view တွင် သင့် floor (ယခုတွင် နံရံများ ပါဝင်သည်) ကို building object ထဲသို့ ဆွဲထည့်ပါ
6.  Window tool ကိုနှိပ်၍ မျက်နှာပြင်ပေါ်တွင် preset တစ်ခုရွေးပြီး နံရံ၏ မျက်နှာပြင်တစ်ခုကို နှိပ်၍ ဦးစားထုတ်ပေါင်းထည့်ပါ
7.  ချိန်ညှိချက်များ ထည့်ရန် လိုအပ်လျှင် အလုပ်လုပ်မည့် plane ကို အရင်သတ်မှတ်ပြီးနောက် Draft Dimension tool ကို အသုံးပြုပါ

အထက်ပါလုပ်ဆောင်မှုများက ဒီပုံစံကို ပေးမည်ဖြစ်သည်။

 <img alt="" src=images/Arch_workflow_example.jpg  style="width:600px;"> 

[ Tutorials](Tutorials.md) စာမျက်နှာတွင် ပိုမိုသိရှိနိုင်သည်။

## Addons

အသုံးပြုသူ တစ်ဦးချင်းစီသည် ဖရီးကက် (FreeCAD) အတွက် မိမိ၏ နယူး features များကို ဖန်တီးပြီး ဖရီးကက် (FreeCAD) အသိုင်းအဝိုင်းနှင့် [addon](Addon.md) အဖြစ် မျှဝေပေးနိုင်သည်။

addon များမှာ အမျိုးသုံးမျိုး ရှိသည် -

-   [Macros](Macros.md): `.FCMacro` ဖြင့် အဆုံးသတ်သည့် ဖိုင်တစ်ဖိုင်အဖြစ် ရှိသော အတိုချုံး [Python](Python.md) ကုဒ် စာပိုဒ်တစ်ပိုဒ်ဖြစ်ပြီး အသစ်သော ကိရိယာ သို့မဟုတ် လုပ်ဆောင်ချက်ကို ပေးသည်။
-   [Workbenches](External_workbenches.md): ထူးခြားသော ခေါင်းစဉ်တစ်ခုကို အလယ်အလတ်ထား၍ ဆက်စပ် [Gui Commands](Gui_Command.md) (ကိရိယာများ) ပေးသည့် Python ဖိုင်စုစည်းမှုများ။
-   [Preference Packs](Preference_Packs.md): အသုံးပြုသူ ပရိသတ်များကို ဖြန့်ချိနိုင်သည့် preference များစုစည်းချက်များ။

## Scripting

နောက်ဆုံးတွင်၊ ဖရီးကက် (FreeCAD) ၏ အားသာဆုံး feature များထဲမှ တစ်ခုမှာ [scripting](Power_users_hub#Scripting_in_FreeCAD.md) ပတ်ဝန်းကျင်ဖြစ်သည်။ တစ်ထောင်ပေါင်းမဟုတ်သော geïntegre Python console မှ (သို့) အခြား Python script များမှ ကြားတွင် သင့်အား ဖရီးကက် (FreeCAD) ၏ အပေါင်းအစုံထိ ဝင်ရောက်နိုင်စေသည်၊ ဂျီယိုမက်ထရီ ဖန်တီးခြင်း သို့မဟုတ် ပြောင်းလဲခြင်း၊ 3D ရုပ်ရှင်တွင် ထို objects များ၏ ကိုယ်ပုံကို ပြောင်းခြင်း သို့မဟုတ် ဖရီးကက် (FreeCAD) အင်တာဖေ့စ်ကို ဝင်ရောက်ပြောင်းလဲနိုင်သည်။ Python scripting ကိုလည်း [macros](macros.md) တွင်အသုံးပြုနိုင်ပြီး၊ ၎င်းက ကွက်တိကျစွာ ကိုယ်ပိုင် command များဖန်တီးရန် လွယ်ကူသောနည်းလမ်းတစ်ခုဖြစ်သည်။

## What's new 

-   အသေးစိတ် feature စာရင်းအတွက် [release notes](Feature_list#Release_notes.md) ကို ကြည့်ပါ။



---
⏵ [documentation index](../README.md) > Getting started