 TutorialInfo:
   Topic:  Drafting
   Level:  Beginner
   Time:  30 minutes
   Author: http://freecadweb.org/wiki/index.php?title=User:Drei Drei and vocx
   FCVersion: 0.19
   Files: https://forum.freecadweb.org/viewtopic.php?f=36&t=43651 Draft tutorial updated
---

# Draft tutorial

 



## အIntroductions

ဤသင်ခန်းစာကို မူရင်းရေးသားခဲ့သူမှာ Drei ဖြစ်ပြီး၊ vocx က ဤကို ပြန်လည်ရေးသား၍ ပုံမှန်သရုပ်ပြထားပါသည်။

ဤသင်ခန်းစာသည် ဖတ်ရှုသူအား <img alt="" src=images/Workbench_Draft.svg  style="width:24px;"> [Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) ၏ မူလလုပ်ဆောင်မှုစဉ်ကို မိတ်ဆက်ပေးရန် ရည်ရွယ်ပါသည်။

ဖတ်ရှုသူမှာ အောက်ပါများကို လက်တွေ့ပြုသန်းလေ့ကျင့်မည်ဖြစ်သည်။

-   ကမ်းလှမ်းရန် လိုအပ်သော သတ်မှတ်ချက်များဖြင့် ကြောင်းများ၊ အကြောင်းဝက်များနှင့် ပုံစံများ ဖန်တီးခြင်း
-   working plane များ၏ အသုံးပြုမှု
-   အတိုင်းအတာများ၊ စာသားများနှင့် ShapeString များ ဖန်တီးခြင်း
-   နည်းပညာရေးဆွဲပုံ (technical drawing) တစ်ခု ဖန်တီးခြင်း

ဤသင်ခန်းစာတွင် {{Value|(x, y, z)}} ဆိုသော သတ်မှတ်ချက်ကို အရာဝတ္ထုအတွင်း အချက်အလက်များကို သတ်မှတ်ရန်ကုဒ်အဖြစ် အသုံးပြုထားသည်။ ပုံမှန်ယူနစ်မှာ မီလီမီတာ {{Value|mm}} ဖြစ်သည်။

 <img alt="" src=images/00_Dr01_Draft_Tutorial_final.png  style="width:" height="400px;">  
*နောက်ဆုံးရေးဆွဲပြီး Draft အရာဝတ္ထုမျိုးစုံပါဝင်သည့် အထွေထွေ ပုံကြမ်း။*

## ဖြန့်ချိရန် စီစဉ်မိန့်

1\. ဖရီးကက် (FreeCAD) ကို ဖွင့်၍ **File → [<img src=images/Std_New.svg style="width:16px"> [New](Std_New.md)** ဖြင့် အလွတ်စာရွက်အသစ်တစ်ခု ဖန်တီးပါ။

:   1.1. [workbench selector](Std_Workbench.md) နှင့်တစ်ပြိုင်နက် သို့မဟုတ် မီနူး **View → Workbench → [<img src=images/Workbench_Draft.svg style="width:16px"> Draft** မှတဆင့် [Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) သို့ ပြောင်းပါ။
:   1.2. [property editor](property_editor.md) (property editor — ပိုင်ဆိုင်မှု တည်းဖြတ်ကိရိယာ) ကို မူကြမ်းနားလည်ပေါက်ပါစေ၊ အထူးသဖြင့် ပိုင်ဆိုင်မှုများပြင်ဆင်ရာတွင် အသုံးပြုသော **Data** နှင့် **View** တက်များကို လေ့လာပါ။ ကုန်ကျစရိတ်များကို ပြောင်းလဲလျှင် [3D view](3D_view.md) (3D မြင်ကွင်း) တွင် ရလဒ်ကို မြင်ရန် **<img src="images/Std_Refresh.svg" width=16px> [Std Refresh](Std_Refresh.md)** အခါတစ်ခါ ပြုလုပ်ရနိုင်ပါသည်။
:   1.3. Draft အရာဝတ္ထုများသည် ပလိန်နာ ပုံစံများ ဖြစ်သဖြင့် ထိပ်မြင်ကွင်းမှ ကြည့်ရသင့်သည်။ [3D view](3D_view.md) ကို ဆက်တင်ရန် **[<img src=images/Std_ViewTop.svg style="width:16px"> [View top](Std_ViewTop.md)** ကို အသုံးပြုပါ။
:   1.4. ဤသင်ခန်းစာတွင် မသုံးခဲ့ပေမယ့် Draft grid သည် ဂျော်မီတရီကွန်ယက်များကို တိကျစွာ တည်နေရာချရန် အထောက်အကူပြုသည်။ [SelectPlane](Draft_SelectPlane.md) ကိုအသုံးပြု၍ working plane နှင့် grid ကို သတ်မှတ်နိုင်ပြီး **[<img src=images/Draft_ToggleGrid.svg style="width:16px"> [Toggle grid](Draft_ToggleGrid.md)** ဖြင့် grid ကို ဖျောက်/ပြသ လုပ်နိုင်ပါသည်။

## Snap toolbar 

2\. [Draft Snap toolbar](Draft_Snap.md) သည် ပုံမှန်အားဖြင့် [Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) သို့ ပြောင်းလဲသည့်အခါ အချိန်နှင့်တပြေးညီ ဖွင့်လှစ်ထားသည်။

:   2.1. အမြဲရှိနေစေရန် [Draft Preferences](Draft_Preferences.md) (Edit → Preferences → Draft → Grid and snapping tab) သို့ သွားပါ။
:   2.2. **Show Draft Snap toolbar** ကို ဖွင့်ထားပြီးဖြစ်ကြောင်း အတည်ပြုပါ။

ဤတည်းက မည်သို့မဆို Draft grid ၏ မြင်နိုင်မှုနှင့် ပိုင်ဆိုင်မှုများကိုပါ တည်းဖြတ်နိုင်သည်။

## Working planes 

Draft အများစုအရာဝတ္ထုများသည် ပလိန်နာ ပုံစံများဖြစ်၍ သဘာဝကျစွာ **working plane** တစ်ခုအပေါ် တည်ဆောက်ထားသည်။ working plane သည် ကမ္ဘာလုံးဆိုင်ရာ ဗဟိုတည်နေရာ XY, XZ, YZ အချင်းအနှောင့် plane များထဲမှ တစ်ခု ဖြစ်နိုင်သလို၊ ၎င်းတို့နှင့် ပါရာလယ်လီယ်ဖြစ်၍ အက်ဖ်စက် (offset) ရှိသော plane ဖြစ်နိုင်သည်၊ သို့မဟုတ် သံလိုက်တစ်ခု၏ မျက်နှာပြင်ဖြင့် သတ်မှတ်ထားသည့် plane ဖြစ်နိုင်ပါသည်။

3\. **[<img src=images/Draft_SelectPlane.svg style="width:16px"> [SelectPlane](Draft_SelectPlane.md)** ကိုနှိပ်ပါ၊ ဒါမှမဟုတ် မီနူး **Utilities → [<img src=images/Draft_SelectPlane.svg style="width:16px"> [Select plane](Draft_SelectPlane.md)** ကိုသွား၍ working plane အတွက် [task panel](task_panel.md) (လုပ်ငန်းတာဝန်ပြား) ကို ဖွင့်ပါ။

:   3.1. **[<img src=images/Std_ViewTop.svg style="width:16px"> Top (XY)** ကို နှိပ်ပါ။

ခလုတ်ကို နှိပ်မည့်အခါ အက်ဖ်စက် (offset) ကို မီလီမီတာအဖြစ်၊ grid spacing၊ main lines နှင့် snapping radius တို့ကို ပြောင်းလဲနိုင်ပါသည်။

## Lines and arcs 

4\. အခု ကျွန်တော်တို့သည် အကြောင်းဝက်များနှင့် ကြောင်းများ ဖန်တီးမည်။

:   4.1. **[<img src=images/Draft_Arc.svg style="width:16px"> [Arc](Draft_Arc.md)** ကို နှိပ်ပါ။
:   4.2. **Center** ကို {{Value|(0, 0, 0)}} အဖြစ် သတ်မှတ်ပြီး **Enter** ကို နှိပ်ပါ။
:   4.3. **Radius** ကို {{Value|30 mm}} အဖြစ် သတ်မှတ်ပြီး **Enter** ကို နှိပ်ပါ။
:   4.4. **Start angle** ကို {{Value|60.0°}} အဖြစ် သတ်မှတ်ပြီး **Enter** ကို နှိပ်ပါ။
:   4.5. **Aperture angle** ကို {{Value|60.0°}} အဖြစ် သတ်မှတ်ပြီး **Enter** ကို နှိပ်ပါ။
:   4.6. အခြား arc တစ် ခုကို radius ကို {{Value|25 mm}} ဖြင့် အထက်ပါ နည်းလမ်းအတိုင်း ထပ်လုပ်ပါ၊ အခြားပုံစံများမှာ ထပ်တူတူဖြစ်သည်။

5\. ယခု ကျွန်တော်တို့သည် arc များကို ကြောင်းများဖြင့် ဆက်သွယ်ကာ ပိတ်ပုံစံ တစ်ခု ဖန်တီးသွားမည်။

:   5.1. **[<img src=images/Draft_Line.svg style="width:16px"> [Line](Draft_Line.md)** ကို နှိပ်ပါ။
:   5.2. [Snap toolbar](Draft_Snap.md) ထဲ၌ **[<img src=images/Draft_Snap_Lock.svg style="width:16px"> [Toggle snap](Draft_Snap_Lock.md)** ကို ဖွင့်ထားပြီး **[<img src=images/Draft_Snap_Endpoint.svg style="width:16px"> [Endpoint](Draft_Snap_Endpoint.md)** ကိုသာ ဖွင့်ထားပါ။ အရွှေ့ပြားကို arc ပေါ်သို့ တပ်မက်သောအခါ arc ၏ endpoint အနီးသို့ ရောက်သည်နှင့် <img alt="" src=images/Draft_Snap_Endpoint.svg  style="width:24px;"> [Endpoint](Draft_Snap_Endpoint.md) icon ပေါ်လာမည်။ အလယ်ဖြင့် ပြည့်စုံသော အဖြစ်ဖြင့် အဖြစ်ရှေ့မှာ ထားရှိထားသော လက်ချက်ဖြင့် အစမ်းနှိပ်၍ စာရင်းကို စတင်ရန် အချက်ကို ရွေးချယ်ပါ။
:   5.3. မျိုးစုံ arc ၏ နီးที่สุด endpoint သို့ မာ့ခ်ကာ နှိပ်၍ arc နှစ်ခုကို ဆက်သွယ်ပါ။
:   5.4. ပရိုဖိုင်ကို ပိတ်ရန် arc ၏ အခြားဘက်အတွက်လည်း အတူတူလုပ်ဆောင်ပါ။

 <img alt="" src=images/01_Dr01_Draft_Arc_profile.png  style="width:" height="400px;">  
*Arc နှစ်ခုနှင့် ကြောင်းနှစ်ခုဖြင့် ပိတ်ထားသည့် ပရိုဖိုင်။*

## Fusing or compounding 

ယခု ကျွန်တော်တို့တွင် [tree view](tree_view.md) (tree မြင်ကွင်း) ထဲတွင် ပိတ်ပုံစံ တစ်ခုကို ဖွဲ့စည်းထားသည့် အရာဝတ္ထု အမျိုးမျိုး ရှိသေးသည်။ သို့သော် ဤပရိုဖိုင်သည် ဆက်စပ်မရှိသေးသော အရာဝတ္ထုများမှ ဖွဲ့စည်းထားသဖြင့် တစ်ခုချင်းစီကို လွတ်လပ်စွာ ပြင်ဆင်ခြင်းနှင့် ရွှေ့ပြောင်းခြင်းများ ပြုလုပ်နိုင်ပါသည်။ ဤအရာများကို ထပ်မံဆက်လက် လုပ်ဆောင်လို့ရသည်၊ သို့သော် အရာများကို တစ်ခုတည်းသော အရာတစ်ခုအဖြစ် အတူပေါင်း၍ fuse လုပ်နိုင်ပါသည်။

6a. အရာများကို တစ်ခုတည်းသို့ fuse လုပ်ခြင်းဖြင့် အဆိုပါ အရာသည် နောက်ထပ် parametric မဟုတ်သော အရာတစ်ခု ဖြစ်လာမည်ဖြစ်၍ ၎င်းတို့၏ properties များကို နောက်ထပ် ပြင်ဆင်လို၍မရတော့ပါ။

:   6a.1. [tree view](tree_view.md) တွင် အရာများလေးခုအားလုံးကို ရွေးချယ်ပါ၊ ဒါမှမဟုတ် **Ctrl** ကို ဖိထား၍ [3D view](3D_view.md) တွင် တစ်ခုချင်းစီကို နှိပ်ရွေးပါ။
:   6a.2. အရာများရွေးထားသောအနေဖြင့် **[<img src=images/Draft_Upgrade.svg style="width:16px"> [Upgrade](Draft_Upgrade.md)** ကို နှိပ်ပါ။
:   6a.3. ၎င်းက အရာလေးခုကို တစ်ခုတည်းသော {{Value|Wire}} အဖြစ် upgrade ပြုလုပ်မည် ဖြစ်ပါသည်။

6b. အရာများ၏ parametric လက္ခဏာကို ထိန်းသိမ်းလိုပါက compound တစ်ခု ဖန်တီးနိုင်ပါသည်။

:   6b.1. <img alt="" src=images/Workbench_Part.svg  style="width:24px;"> [Part Workbench](Part_Workbench.md) (Part Workbench — အပိုင်း လုပ်ငန်းခွင်) သို့ ပြောင်းပါ။
:   6b.2. အရာများရွေးထားသောအနေဖြင့် **[<img src=images/Part_Compound.svg style="width:16px"> [Part Compound](Part_Compound.md)** ကို နှိပ်ပါ။

## Rectangles, circles, and polygons 

7\. အခု ကျွန်တော်တို့ rectangular frame တစ်ခု ဆွဲမည်။ (ပြန်လည် <img alt="" src=images/Workbench_Draft.svg  style="width:24px;"> [ Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) သို့ ပြောင်းပါ။)

:   7.1. **[<img src=images/Draft_Rectangle.svg style="width:16px"> [Rectangle](Draft_Rectangle.md)** ကို နှိပ်ပါ။
:   7.2. ပထမအမှတ်နေရာကို {{Value|(-100, -60, 0)}} ထည့်ပြီး **Enter** ကို နှိပ်ပါ။
:   7.3. အချက်အလက်အတွက် **Relative** ရွေးချယ်မှုကို uncheck ထားပါ၊ ကျွန်တော်တို့သည် absolute ဥစ္စာတန်ဖိုးများကို သုံးမည်ဖြစ်သည်။ အမြန် toggle ပြန်လွှေအောင် ကီးဘုတ်ပေါ်မှ **R** ကို နိုပ်နိုင်သည်။
:   7.4. ဒုတိယအမှတ်နေရာ၏ ကိန်းဂဏန်းကို {{Value|(140, 90, 0)}} ထည့်ပြီး **Enter** ကို နှိပ်ပါ။

Rectangle တစ်ခု ဖန်တီးပြီးပါပြီ။ ၎င်း၏ properties များကို ပြောင်းရန် [property editor](Property_editor.md) (property editor — ပိုင်ဆိုင်မှု တည်းဖြတ်ကိရိယာ) သို့ သွားကြည့်ပါ။ rectangle သည် face ဖန်တီး မဖြစ်စေလိုပါက **Make Face** ကို `False` သို့ သတ်မှတ်ပါ။ face ဖန်တီးချင်ပြီးလည်း အဲဒီ object ၏ wires များသာ မြင်ချင်ပါက **Make Face** ကို `True` ထားပြီး **Display Mode** ကို {{Value|Wireframe}} သို့ သတ်မှတ်ပါ။

8\. ငါတို့က circle တစ်ခု ဆွဲမည်။

:   8.1. **[<img src=images/Draft_Circle.svg style="width:16px"> [Circle](Draft_Circle.md)** ကို နှိပ်ပါ။
:   8.2. center အတွက် {{Value|(0, 0, 0)}} ထည့်၍ **Enter** ကို နှိပ်ပါ။
:   8.3. radius ကို {{value|15 mm}} သတ်မှတ်ပြီး **Enter** ကို နှိပ်ပါ။

9\. မကြာခဏနှင့်ရှိသည့် polygon တစ်ခု ဆွဲမည်။

:   9.1. **[<img src=images/Draft_Polygon.svg style="width:16px"> [Polygon](Draft_Polygon.md)** ကို နှိပ်ပါ။
:   9.2. center အတွက် {{Value|(0, 0, 0)}} ထည့်၍ **Enter** ကို နှိပ်ပါ။
:   9.3. number of sides ကို {{Value|6}} သတ်မှတ်၍ **Enter** ကို နှိပ်ပါ။
:   9.4. radius ကို {{Value|50 mm}} သတ်မှတ်၍ **Enter** ကို နှိပ်ပါ။

ပြန်လည် [property editor](property_editor.md) (property editor — ပိုင်ဆိုင်မှု တည်းဖြတ်ကိရိယာ) တွင် **Make Face** နှင့် **Display Mode** အချက်များကို လိုအပ်သလို ပြင်ဆင်နိုင်သည်။

Rectangle, circle, polygon နှင့် [Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) မှ ဖန်တီးသည့် အခြားအရာဝတ္ထုအများစုသည် base class ဖြစ်သည့် [Part Part2DObject](Part_Part2DObject.md) မှ ဆင်းသက်လာသောကြောင့် data နှင့် view properties များကိုမျှဝေကြသည်။

 <img alt="" src=images/02_Dr01_Draft_Rectangle_circle_polygon.png  style="width:" height="400px;">  
*Rectangle, circle နှင့် polygon ထည့်သွင်းပြီး။*

## Arrays

Arrays များကို အရာဝတ္ထုတစ်ခုကို အနောက်/ဘယ်/ညာ (X, Y, Z) လမ်းကြောင်းများဖြင့် မျှတစွာ many replicate လုပ်ရန်၊ revolution axis အပေါ် ပတ်၍တက်ရန်၊ သို့မဟုတ် path တစ်ခုလိုက်၍ replicate လုပ်ရန် အသုံးပြုသည်။

10\. Polar array တစ်ခု ဖန်တီးမည်။

:   10.1. အရင်ဆုံး **[<img src=images/Draft_Upgrade.svg style="width:16px"> [Upgrade](Draft_Upgrade.md)** ကိရိယာဖြင့် ဖန်တီးခဲ့သော {{Value|Wire}} object ကို ရွေးချယ်ပါ၊ ဒါမှမဟုတ် **[<img src=images/Part_Compound.svg style="width:16px"> [Part Compound](Part_Compound.md)** ဖြင့် ဖန်တီးထားသော {{Value|Compound}} ကို ရွေးချယ်ပါ။
:   10.2. **[<img src=images/Draft_PolarArray.svg style="width:16px"> [PolarArray](Draft_PolarArray.md)** ကို နှိပ်ပါ။
:   10.3. polar angle ကို {{Value|360°}} သတ်မှတ်ပါ။
:   10.4. elements အရေအတွက်ကို {{Value|4}} သတ်မှတ်ပါ။
:   10.5. အနုတ်လှည့်စက်၏ center အနေဖြင့် {{Value|(0, 0, 0)}} ထည့်၍ **Enter** ကို နှိပ်ပါ။

Array object သည် origin အနီးတွင် အရာ၏ ကူးပြောင်းများကို ပြသပါလိမ့်မည်။

 <img alt="" src=images/03_Dr01_Draft_PolarArray.png  style="width:" height="400px;">  
*origin အနီး၌ ဗဟိုထားသော ကျွန်တော်တို့၏ သေးငယ်သော ပရိုဖိုင်၏ polar array။*

## Dimensions

Linear dimensions များသည် အတိုင်းအတာများကို တိုင်းတာရန် [Draft Snap](Draft_Snap.md) ၏ သင့်လျော်သော ချိတ်ဆက်မှုများကို အသုံးပြုသည့်အခါ ကောင်းမွန်စွာ လုပ်ဆောင်နိုင်သည်။ သို့သော် absolute coordinates ကို သတ်မှတ်ကာလည်း ဖန်တီးနိုင်သည်။

11\. အမျိုးမျိုးသော အရာဝတ္ထုများအတွက် dimension များ ဖန်တီးပါ။

:   11.1. **[<img src=images/Draft_Dimension.svg style="width:16px"> [Dimension](Draft_Dimension.md)** ကို နှိပ်ပါ။
:   11.2. ပထမအမှတ်ကို ရွေးချယ်ပါ။ ဤသင်ခန်းစာတွင် ပထမအမှတ်မှာ အမြဲ မြစ်၏ origin {{Value|(0, 0, 0)}} ဖြစ်ပါမည်။
:   11.3. [Snap toolbar](Draft_Snap.md) ထဲ၌ **[<img src=images/Draft_Snap_Lock.svg style="width:16px"> [Toggle snap](Draft_Snap_Lock.md)** ကို ဖွင့်ထားပြီး **[<img src=images/Draft_Snap_Midpoint.svg style="width:16px"> [Midpoint](Draft_Snap_Midpoint.md)** ကိုသာ ဖွင့်ထားပါ။ pointer ကို polygon ၏ အပေါ် အရိုးသို့ ရွှေ့သွားသောအခါ <img alt="" src=images/Draft_Snap_Midpoint.svg  style="width:24px;"> [Midpoint](Draft_Snap_Midpoint.md) icon ပေါ်လာမည်။ ဤနေရာကို နှိပ်၍ ရွေးပါ။
:   11.4. dimension တည်နေရာကို သတ်မှတ်ရန် cursor ကိုညာဘက်သို့ ရွှေ့ပြီး သုံးချက်နှိပ်ပါ၊ အနီးကပ် {{Value|(100, 20, 0)}} အနီးတွင် ထားပါ။ dimension သည် အလိုအလျောက် နှစ်ကြားရှိအကွာအဝေးကို ပြချက်ပြမည်။
:   11.5. [tree view](tree_view.md) တွင် dimension object ကို ရွေးပြီး [property editor](Property_editor.md) (property editor — ပိုင်ဆိုင်မှု တည်းဖြတ်ကိရိယာ) ထဲတွင် **Font Size** ကို {{Value|6 mm}} သို့ ပြောင်းပါ၊ **Ext Lines** ကို {{Value|45 mm}} သတ်မှတ်ပါ၊ နှင့် **Show Unit** ကို `False` သတ်မှတ်ပါ။

12\. ပိတ်ထားသော ပရိုဖိုင်၏ နှစ်ခုသော arc များအတွက်လည်း ထပ်လုပ်ပါ။ တိုင်းတာမှု၏ ပထမအမှတ်မှာ မျှော်လင့်သလို origin ဖြစ်မည်၊ ဒုတိယအမှတ်မှာ arc ၏ <img alt="" src=images/Draft_Snap_Midpoint.svg  style="width:24px;"> [Midpoint](Draft_Snap_Midpoint.md) သည် ဖြစ်မည်။

13\. အလယ်တွင် တည်ရှိသည့် circle အတွက်လည်း ထပ်လုပ်ပါ။ တိုင်းတာမှု၏ ပထမအမှတ်မှာ ဆက်လက် origin ဖြစ်မည်။ ဒုတိယအမှတ်ကို ရွေးရန် **[<img src=images/Draft_Snap_Lock.svg style="width:16px"> [Toggle snap](Draft_Snap_Lock.md)** ကို ဖွင့်ထားပြီး **[<img src=images/Draft_Snap_Angle.svg style="width:16px"> [Angle](Draft_Snap_Angle.md)** ကိုသာ ဖွင့်ပါ။ pointer ကို circle ၏ ထိပ်သို့ ရွှေ့သို့ချိန် <img alt="" src=images/Draft_Snap_Angle.svg  style="width:24px;"> [Angle](Draft_Snap_Angle.md) icon ပေါ်လာမည်၊ ထိုနေရာကို နှိပ်၍ ရွေးချယ်ပါ။ ထို့နောက် cursor ကိုညာဘက်သို့ ရွှေ့ပြီး dimension ကို အတည်ပြုရန် နှိပ်ပါ။

dimension ကို မှန်ကန်စွာ မြင်ရန် **Font Size** နှင့် အခြား properties များကို ပြင်ပါ။

 <img alt="" src=images/04_Dr01_Draft_Dimension.png  style="width:" height="400px;">  
*Dimension များသည် origin မှ circle, arc နှင့် polygon ၏ ထိပ်ထိမှတ်အထိ ညီထပ်မျှ အလျားအဝေးကို တိုင်းတာပြသည်။*

## Texts and ShapeStrings 

14\. Text objects များသည် ပလိန်နာ ပုံစံရိယာများ ဖြစ်ကြပြီး [3D view](3D_view.md) (3D မြင်ကွင်း) တွင် ဖန်တီးရသော်လည်း အောက်ခံတွင် အမှန်တကယ် “[shape](Shape.md)” မရှိပါ။ ၎င်းသည် သူတို့အား extrusions သို့မဟုတ် boolean လုပ်ဆောင်ချက်များကဲ့သို့သော ရှယ်ပိတ်လှုပ်ရှားမှုများတွင်အသုံးမပြုနိုင်စေရန် ဖြစ်သည်။

:   14.1. **[<img src=images/Draft_Text.svg style="width:16px"> [Text](Draft_Text.md)** ကို နှိပ်ပါ။
:   14.2. [3D view](3D_view.md) တွင် reference point ကို ရွေးချယ်ပါ။ [Snap toolbar](Draft_Snap.md) ထဲ၌ **[<img src=images/Draft_Snap_Lock.svg style="width:16px"> [Toggle snap](Draft_Snap_Lock.md)** ကို ဖွင့်ထားပြီး **[<img src=images/Draft_Snap_Midpoint.svg style="width:16px"> [Midpoint](Draft_Snap_Midpoint.md)** ကိုသာ ဖွင့်ထားပါ။ pointer ကို အကြီးဆုံး arc ၏ အပေါ်ဘက် အရိုးသို့ ရွှေ့ပါ၊ အချိန်နှင့်တကွ <img alt="" src=images/Draft_Snap_Midpoint.svg  style="width:24px;"> [Midpoint](Draft_Snap_Midpoint.md) icon ပေါ်လာမည်၊ ထိုနေရာကို နှိပ်၍ ရွေးပါ။
:   14.3. လိုချင်သည့် **Text** ကို ထည့်၍ မျက်နှာသစ်စတင်ရန် မျက်နှာသစ်တစ်ကြောင်းစတင်ရန် **Enter** တစ်ခါနှိပ်ပါ၊ လိုအပ်သလို အခြားကြောင်းများ ထပ်ထည့်နိုင်သည်။
:   14.4. ပြီးဆုံး၍ ပြင်ဆင်မှုကို ရပ်တန့်လိုပါက **Enter** ကို နှစ်ချက် နှိပ်ပါ။
:   14.5. [tree view](tree_view.md) တွင် text object ကို ရွေးပြီး [property editor](Property_editor.md) (property editor — ပိုင်ဆိုင်မှု တည်းဖြတ်ကိရိယာ) တွင် **Font Size** ကို {{Value|6 mm}} သတ်မှတ်ပြီး **Justification** ကို {{Value|Center}} သို့ ပြောင်းပါ။

15\. ShapeString objects များမှာ ကုဒ်ထိုးထားသည့် ဖောင့်တစ်ခုအရ လိုင်းများကို လိုက်နာထားသော primitive wire များဖြင့် ဖွဲ့ထားသည့် shapes ဖြစ်ကြသည်။ ၎င်းတို့တွင် အောက်ခံ “[shape](Shape.md)” တကယ် ရှိသည် ဆိုတော့ extrusion သို့မဟုတ် boolean လုပ်ဆောင်ချက်များကဲ့သို့သော UIs တွင် အသုံးပြုနိုင်ပါသည်။

:   15.1. **[<img src=images/Draft_ShapeString.svg style="width:16px"> [ShapeString](Draft_ShapeString.md)** ကို နှိပ်ပါ။
:   15.2. [3D view](3D_view.md) တွင် regular polygon အထက်မွန်းကပ်သော တည်နေရာတွင် pointer ကို ရွှေ့ပြီး တစ်ချက် နှိပ်ပါ။ ၎င်းသည် ShapeString အတွက် base point ကို သတ်မှတ်မည်။ ကိန်းဂဏန်းများကိုလည်း လက်ဖြင့် ထည့်နိုင်ပြီး ဥပမာအနေဖြင့် {{Value|(-20, 65, 0)}} ဟုတ်သည်။
:   15.3. လိုချင်သည့် **String** ကို ထည့်ပြီး လိုအပ်သည့် **Height** ကို ရွေးပါ။
:   15.4. default font file မရှိပါက ellipsis **...** ကို နှိပ်၍ စနစ်အတွင်းမှ font ဖိုင်လိပ်စာကို ရွေးချယ်ရန် dialog box ကို ဖွင့်ရမည်။
:   15.5. မှန်ကန်သည့် font file ကို သတ်မှတ်ပြီးပါက **OK** ကို နှိပ်ပါ သို့မဟုတ် **Enter** ကို နှိပ်၍ ဆက်သွားနိုင်သည်။

 <img alt="" src=images/05_Dr01_Draft_Text_ShapeString.png  style="width:" height="400px;">  
*Text နှင့် ShapeString objects များ ထည့်သွင်းပြီး။*

စာလုံးများကို extrude လုပ်၍ သတ္တုပစ္စည်းပေါ်တွင် သွေးရိုက်လိုပါက [Draft ShapeString tutorial](Draft_ShapeString_tutorial.md) ကို ကြည့်ပါ။

## နည်းပညာရေးဆွဲပုံများ ဖန်တီးခြင်း 

ယခုအခါ ဖန်တီးထားသည့် အရာဝတ္ထုများကို သိမ်းဆည်းနိုင်ပြီး၊ [SVG](SVG.md) သို့မဟုတ် [DXF](DXF.md) ကဲ့သို့ အခြားဖိုင်ဖော်မက်များသို့ export ပြုလုပ်နိုင်၊ သို့မဟုတ် ပရင့်ထုတ်နိုင်ပါသည်။

လိုပါက ဤအရာများကို frame ကဲ့သို့သော ထည့်သွင်းချက်များနှင့် အတူ ပြသရန် နည်းပညာရေးဆွဲပုံ (technical drawing) တစ်ခု ဖန်တီးနိုင်သည်။

မည်သည့် အရာမျှမ ပြုလုပ်မီ Draft grid ကို ဖျောက်ရန် **[<img src=images/Draft_ToggleGrid.svg style="width:16px"> [Toggle  grid](Draft_ToggleGrid.md)** ကို နှိပ်ပါ။

16\. <img alt="" src=images/Workbench_TechDraw.svg  style="width:24px;"> [TechDraw Workbench](TechDraw_Workbench.md) (TechDraw Workbench — TechDraw လုပ်ငန်းခွင်) သို့ ပြောင်းပါ။

:   16.1. **[<img src=images/TechDraw_PageDefault.svg style="width:16px"> [TechDraw PageDefault](TechDraw_PageDefault.md)** ကို နှိပ်ပြီး စံပြစာမျက်နှာတစ်ခု ဖန်တီးပါ။
:   16.2. [tree view](tree_view.md) ထဲမှ Page ကို 제외၍ ဖန်တီးထားသည့် အရာများအားလုံးကို ရွေးချယ်ပြီး **[<img src=images/TechDraw_ActiveView.svg style="width:16px"> [TechDraw ActiveView](TechDraw_ActiveView.md)** ကို နှိပ်ပါ။ default options ဖြင့် **OK** ကို နှိပ်ပါ၊ စာမျက်နှာအတွင်း view တစ်ခု ဖန်တီးရန် နာရီတစ်စက္ကန့် စောင့်ရနိုင်သည်။
:   16.3. [tree view](tree_view.md) တွင် Page object ကို ရွေးချယ်ခြင်းဖြင့် Page သည် မူလပြင်တွင် မျက်နှာပေါ် ပြသမည်။ Page ကို ရွေးထားစဉ် [property editor](Property_editor.md) (property editor — ပိုင်ဆိုင်မှု တည်းဖြတ်ကိရိယာ) တွင် **Scale** ကို {{Value|0.75}} သို့ ပြောင်းပါ။
:   16.4. [tree view](tree_view.md) တွင် Page object ကို တိုးချဲ့၍ ActiveView object ကို ရွေးပါ။ ဤ view ကို ရွေးထားစဉ် [property editor](Property_editor.md) တွင် **Scale Type** ကို {{Value|Page}} သို့ ပြောင်းပါ။
:   16.5. **[<img src=images/Std_Refresh.svg style="width:16px"> [Refresh](Std_Refresh.md)** သို့မဟုတ် F5 ကို နှိပ်၍ မော်ဒယ်ကို ပြန်တွက်ပါ။
:   16.6. အရာဝတ္ထုများ၏ ဖရိမ်ကို ဖျောက်ရန် **[<img src=images/TechDraw_ToggleFrame.svg style="width:16px"> [TechDraw ToggleFrame](TechDraw_ToggleFrame.md)** ကို နှိပ်ပါ။

[TechDraw Workbench](TechDraw_Workbench.md) ကို ပိုမိုလေ့လာလိုပါက [Basic TechDraw Tutorial](Basic_TechDraw_Tutorial.md) ကို ဖတ်ရှုပါ။

 <img alt="" src=images/06_Dr01_Draft_TechDraw_page.png  style="width:" height="400px;">  
*Draft Workbench ဖြင့် ဖန်တီးထားသည့် shapes များကို projection အဖြစ် ထည့်သည့် TechDraw စာမျက်နှာ။*

TechDraw သည် [Part TopoShape](Part_TopoShape.md) ရှိသော အရာများနှင့် ပို၍ ကောင်းစွာ လုပ်ဆောင်သည်။ Draft မှာ အချို့ object များ၊ ဥပမာ [Draft Texts](Draft_Text.md) နှင့် [Draft Dimensions](Draft_Dimension.md) ကဲ့သို့သောအရာများတွင် အများအားဖြင့် အဲဒီ “[shapes](Shape.md)” မရှိသောကြောင့် TechDraw ၏ အချို့ လုပ်ဆောင်ချက်များသည် ဤ အရာများနှင့် မအလုပ်လုပ်နိုင်ပါ။

**[<img src=images/TechDraw_ActiveView.svg style="width:16px"> [TechDraw ActiveView](TechDraw_ActiveView.md)**, **[<img src=images/TechDraw_DraftView.svg style="width:16px"> [TechDraw DraftView](TechDraw_DraftView.md)**, နှင့် **[<img src=images/TechDraw_ArchView.svg style="width:16px"> [TechDraw ArchView](TechDraw_ArchView.md)** ကဲ့သို့သော ကိရိယာများသည် Draft ၏ အတွင်းရေး SVG ပုံတစ်ခုကို လက်ခံကာ အဲဒါဖြင့် view များကို ဖန်တီးသည်။ ထို့ကြောင့် TechDraw သည် ဤ view များပြသပုံအပေါ် စနစ်တကျ ထိန်းချုပ်မှုနည်းပါးလျှင် Draft နှင့် TechDraw အနှံ့ပို၍ ပေါင်းစည်းမှုဆောင်ရွက်ရန် အလုပ်များ ဆက်လက်လုပ်ဆောင်နေဆဲ ဖြစ်ပါသည်။

## နောက်ဆုံး မှတ်ချက်များ 

[Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) သည် အများအားဖြင့် [Sketcher Workbench](Sketcher_Workbench.md) (Sketcher — ပုံကြမ်းဖန်တီးမှု) နှစ်ခုစလုံးသည် 2D shapes ဖန်တီးရန် ရည်ရွယ်ထားသည့်အမျိုးအစားဖြစ်သလို ဆင်တူချက်များ ရှိပါသည်။ အဓိက ကွာခြားချက်မှာ workbench တစ်ခုစီ သည် coordinate system များကို မည်သို့ ကိုင်တွယ်ပေးသည့်နည်းနှင့် object များကို မည်သို့ တည်နေရာချထားသည့်နည်း ဖြစ်သည်။ Draft တွင် အရာများကို global coordinate system အတွင်း လွတ်လပ်စွာ တည်နေရာချနိုင်ပြီး ပုံမှန်အားဖြင့် ၎င်း၏ မှတ်ချက်များကို grid သို့မဟုတ် အခြား object များထံ snap လုပ်ကာ အချက်များကို တည်နေရာချသည်။ Sketcher တွင်则 "[sketch object](Sketch.md)" သည် local coordinate system ကို သတ်မှတ်ပေးပြီး အဲဒါသည် sketch အတွင်းရှိ ဂျော်မီတရီအရာများ၏ ရည်ညွှန်းစနစ်အဖြစ် အသုံးပြုသည်။ ထို့ပြင် sketch သည် ၎င်း၏ အချက်များ၏ နောက်ဆုံးတည်နေရာကို သတ်မှတ်ရန် "ကန့်သတ်ချက်များ (constraints)" တွေပေါ် အခြေခံပါသည်။

-   [Draft Workbench](Draft_Workbench.md) (Draft လုပ်ငန်းခွင်) သည် grid မြေပုံပေါ်တွင် ဆွဲရန် သင့်တော်သည့် 2D ရေးဆွဲချက်များအတွက် ရည်ရွယ်ထားသည်။ [BIM Workbench](BIM_Workbench.md) သည် အဓိကအားဖြင့် [Draft Workbench](Draft_Workbench.md) ၌ သတ်မှတ်ထားသည့် ကိရိယာများကို အခြေခံကာ တည်ဆောက်ထားသည်။

-   [Sketcher Workbench](Sketcher_Workbench.md) (Sketcher — ပုံကြမ်းဖန်တီးမှု) သည် အချက်များကြား တိကျသည့် ဆက်စပ်မှုများ လိုအပ်သည့် 2D ရေးဆွဲချက်များအတွက် ရည်ရွယ်ထားသည်။ ၎င်းသည် grid သို့ မီပါသော်လည်း အချက်များနှင့် အနားများထားရာကို သတ်မှတ်ရန် တွက်ချက်မှုများ (constraints) ပေါ်တွင် အထူးလျှောက်ထားသည်။ [Sketcher Workbench](Sketcher_Workbench.md) ကို ပုံမှန်အားဖြင့် [PartDesign Workbench](PartDesign_Workbench.md) (Part Design — အစိတ်အပိုင်း ဒီဇိုင်း) နှင့် တွဲပြီး solid [bodies](Body.md) ဖန်တီးရာတွင် အသုံးပြုကြသည်။

-   Draft object တစ်ခုကို [Sketch](Sketch.md) သို့ပြောင်းနိုင်ပြီး၊ မှီခို၍ **[<img src=images/Draft_Draft2Sketch.svg style="width:16px"> [Draft Draft2Sketch](Draft_Draft2Sketch.md)** ကိရိယာကိုအသုံးပြုကာ အခြားဘက်သို့လည်း ပြန်လည်ပြောင်းနိုင်သည်။



---
⏵ [documentation index](../README.md) > [Draft](Draft_Workbench.md) > Draft tutorial