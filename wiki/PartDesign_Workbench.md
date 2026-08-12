# <img alt="PartDesign workbench icon" src=images/Workbench_PartDesign.svg  style="width:64px;"> အစိတ်အပိုင်း ဒီဇိုင်း လုပ်ငန်းခွင် (PartDesign Workbench)

 

## မိတ်ဆက်

The <img alt="" src=images/Workbench_PartDesign.svg  style="width:32px;"> **အစိတ်အပိုင်း ဒီဇိုင်း လုပ်ငန်းခွင် (PartDesign Workbench)** သည် အထူ (solid) အစိတ်အပိုင်းများကို မော်ဒယ်ဖန်တီးရန် နည်းပညာကိရိယာများကို ပေးဆောင်သည်။ အဓိကအားဖြင့် ထုတ်လုပ်နိုင်ပြီး အစည်းအပဖြစ်အောင် တပ်ဆင်နိုင်သည့် မက်ကန်းနစ် အစိတ်အပိုင်းများ ဖန်တီးရန် အာရုံစိုက်ထားသည်။ သို့သော် ဖန်တီးထားသည့် အထူပစ္စည်းများကို [BIM modeling](BIM_Workbench.md), [finite element analysis](FEM_Workbench.md) သို့မဟုတ် [machining and 3D printing](CAM_Workbench.md) ကဲ့သို့ အခြား ရည်ရွယ်ချက်များအတွက်လည်း အသုံးပြုနိုင်သည်။

  
အစိတ်အပိုင်း ဒီဇိုင်း လုပ်ငန်းခွင်သည် feature-based နည်းလမ်းကို အသုံးပြုသည်။ တစ်ခုသော component ကို Body အရာဝတ္ထု ကွန်တိန်နာဖြင့် ကိုယ်စားပြုထားသည်။ Body သည် ဒေသဆိုင်ရာ ကိုအော်ဒင်နိတ် စနစ် (local coordinate system) ကို သတ်မှတ်ကာ အစိတ်အပိုင်းကို သတ်မှတ်သော စုပေါင်း feature များကို ပါ၀င်ထားသည်။ အများစုသော features များသည် parametric စကစ်များ (parametric sketches) အပေါ် အခြေခံထားပြီး ပေါင်းထည့် (additive) သို့မဟုတ် ဖြုတ်ပစ် (subtractive) ဖြစ်ပြီး အမျိုးအစားများဖြစ်သည်။ ဥပမာအားဖြင့် [Pad tool](PartDesign_Pad.md) သည် အထူထွက်ပေါက်သော စကစ်ကို တည်ဆောက်နေသည့် အထူတွင် ပေါင်းထည့်ပေးပြီး၊ [Pocket tool](PartDesign_Pocket.md) သည် အထူထွက်ပေါက်သော စကစ်ကို ဖြုတ်ပစ်ပေးသည်။ တစ်ခုချင်းစီသော feature တစ်ခုချင်းစီသည် စုပေါင်းဖြစ်ပြီး ကြိုတင်ဖန်တီးထားသော feature များ၏ ရလဒ်ပေါ်တွင် ဆက်လက်တည်ဆောက်သည်။ ထို့အပြင် primitive များ ([Cylinder](PartDesign_AdditiveCylinder.md), [Sphere](PartDesign_AdditiveSphere.md) စသည်) သို့မဟုတ် Body အပြင်တွင် ဖန်တီးထားသော solids များကို feature အဖြစ် အသုံးပြုနိုင်သည်။

ဒီလုပ်ငန်းစဉ်အား ပိုမိုအပြည့်အစုံ ရှင်းလင်းရန် [feature editing](Feature_editing.md) စာမျက်နှာကို ကြည့်ပါ၊ ပြီးလျှင် အချင်းချင်း အထူများ ဖန်တီးရန် စတင်လိုသူများအတွက် [Creating a simple component with PartDesign](Creating_a_simple_part_with_PartDesign.md) ကို ကြည့်ရှုပါ။

The <img alt="" src=images/Workbench_Part.svg  style="width:16px;"> [Part Workbench](Part_Workbench.md) သည် shape များတည်ဆောက်ရန် အတွက် အခြားတစ်မျိုးသော constructive solid geometry (CSG) နည်းလမ်းကို ပေးဆောင်သည်။ Part Workbench နှင့် Part Design Workbench တို့၏ အသေးစိတ် ဆွေးနွေးချက်အတွက် [Part and Part Design](Part_and_PartDesign.md) ကို ကြည့်ပါ။

 ![](images/PartDesign_Workbench_Example.jpg ) 

## ကိရိယာများ

Part Design ကိရိယာများကို မိမိ Part Design လုပ်ငန်းခွင်ကို ဖွင့်သည့်အခါ သင့်အားမြင်နေရမည့် **Part Design** မီနူးနှင့် PartDesign တူးလ်ဘားတို့တွင် တွေ့နိုင်သည်။

### Part Design အကူအညီ ကိရိယာများ 

-   <img alt="" src=images/PartDesign_Body.svg  style="width:32px;"> [Create body](PartDesign_Body.md): လက်ရှိ document တွင် [Body](Body.md) အရာဝတ္ထုတစ်ခုကို ဖန်တီးပြီး active အဖြစ် သတ်မှတ်သည်။

-   <img alt="" src=images/PartDesign_NewSketch.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Create Sketch:

  -<img alt="" src=images/PartDesign_NewSketch.svg  style="width:32px;"> [Create sketch](PartDesign_NewSketch.md): ရွေးချယ်ထားသော မျက်နှာ (face) သို့မဟုတ် ပလိန်းပေါ်တွင် စကစ် အသစ် တစ်ခု ဖန်တီးသည်။ ဒီကိရိယာကို အချိန်ယူ လုပ်ဆောင်သည့်အခါ မည်သည့် မျက်နှာကို မရွေးထားပါက Tasks panel မှ ပလိန်းတစ်ခုကို ရွေးချယ်ရန် အသုံးပြုသူအား မေးမြန်းမည်ဖြစ်သည်။ အင်တာဖေ့စ်သည် စကစ် တည်းဖြတ်မှု မုဒ်ဖြင့် [Sketcher Workbench](Sketcher_Workbench.md) သို့ လွှဲပြောင်းပါလိမ့်မည်။

  - <img alt="" src=images/Sketcher_MapSketch.svg  style="width:32px;"> [Attach sketch](Sketcher_MapSketch.md): လက်ရှိ Body မှ ရွေးချယ်ထားသော ဂျီအိုမက်ထရီ (geometry) သို့ စကစ်ကို တွဲဆက်တပ်ဆင်သည်။

  - <img alt="" src=images/Sketcher_EditSketch.svg  style="width:32px;"> [Edit sketch](Sketcher_EditSketch.md): ရွေးချယ်ထားသော စကစ်ကို တည်းဖြတ်ရန် ဖွင့်သည်။

-   <img alt="" src=images/Sketcher_ValidateSketch.svg  style="width:32px;"> [Validate sketch](Sketcher_ValidateSketch.md): ချက်တိအချက်ပေါင်းများ၏ ချွတ်ယွင်းချက်များကို စစ်ဆေး၍ တိကျမှုကို ညှိနှိုင်းပေးသည်။

-   <img alt="" src=images/Part_CheckGeometry.svg  style="width:32px;"> [Check geometry](Part_CheckGeometry.md): ရွေးထားသော အရာများ၏ ဂျီအိုမက်ထရီကို မှားယွင်းချက်များအတွက် စစ်ဆေးသည်။

-   <img alt="" src=images/PartDesign_ShapeBinder.svg  style="width:32px;"> [Create a shape binder](PartDesign_ShapeBinder.md): မိမိ parent object တစ်ခုမှ ဂျီအိုမက်ထရီကို ကိုးကားသတ်မှတ်သော shape binder တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_SubShapeBinder.svg  style="width:32px;"> [Create a sub-object(s) shape binder](PartDesign_SubShapeBinder.md): parent objects အများအပြားမှ ဂျီအိုမက်ထရီများကို ကိုးကားသတ်မှတ်သည့် shape binder တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_Clone.svg  style="width:32px;"> [Create a clone](PartDesign_Clone.md): ရွေးထားသော Body ၏ ကလုန်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_Plane.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Create a datum (

  -<img alt="" src=images/PartDesign_Plane.svg  style="width:32px;"> [Create a datum plane](PartDesign_Plane.md): လက်ရှိ Body အတွင်း datum plane တစ်ခု ဖန်တီးသည်။ ({{VersionMinus|1.0}})

  -<img alt="" src=images/PartDesign_Line.svg  style="width:32px;"> [Create a datum line](PartDesign_Line.md): လက်ရှိ Body အတွင်း datum line တစ်ခု ဖန်တီးသည်။ ({{VersionMinus|1.0}})

  -<img alt="" src=images/PartDesign_Point.svg  style="width:32px;"> [Create a datum point](PartDesign_Point.md): လက်ရှိ Body အတွင်း datum point တစ်ခု ဖန်တီးသည်။ ({{VersionMinus|1.0}})

  -<img alt="" src=images/PartDesign_CoordinateSystem.svg  style="width:32px;"> [Create a local coordinate system](PartDesign_CoordinateSystem.md): လက်ရှိ Body အတွင်း datum ဂျီအိုမက်ထရီနှင့် တွဲထားသော ဒေသဆိုင်ရာ ကိုအော်ဒင်နိတ်စနစ် တစ်ခု ဖန်တီးသည်။ ({{VersionMinus|1.0}})

:   
    <small>(v1.1)</small> : ဒီကိရိယာများကို အသစ်ပြုလုပ်ထားသည့် [datum tools](Std_Base#Part_Datums.md) များဖြင့် အစားထိုးထားပါသည်။

### Part Design မော်ဒယ်ဖန်တီး ကိရိယာများ 

#### ပေါင်းထည့် ကိရိယာများ (Additive tools)

ဤကိရိယာများသည် အခြေခံ feature များ ဖန်တီးရန် သို့မဟုတ် ရှိပြီးသား Body သို့ ပစ္စည်း (material) ထပ်ထည့်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/PartDesign_Pad.svg  style="width:32px;"> [Pad](PartDesign_Pad.md): ရွေးချယ်ထားသော စကစ်မှ အထူကို extrude ပြုလုပ်၍ အထူတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_Revolution.svg  style="width:32px;"> [Revolution](PartDesign_Revolution.md): စကစ်ကို အက်ဆစ်တစ်ခုအပေါ် လှည့်ပတ်တည်ဆောက်၍ အထူတစ်ခု ဖန်တီးသည်။ စကစ်သည် ပိတ်၍ ပေါင်းစပ်ထားသည့် ပရိုဖိုင်းဖြစ်ရမည်။

-   <img alt="" src=images/PartDesign_AdditiveLoft.svg  style="width:32px;"> [Additive loft](PartDesign_AdditiveLoft.md): နှစ်ခု သို့မဟုတ် ထိုထက်ပိုသော စကစ်များအကြား လှိုင်းပြောင်းသည့် အတည်အမှန်ဖြင့် အထူတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_AdditivePipe.svg  style="width:32px;"> [Additive pipe](PartDesign_AdditivePipe.md): ဖွင့်ထားသည့် သို့မဟုတ် ပိတ်ထားသည့် ပတ်လမ်းတစ်ခုအရ စကစ်တစ်ခု (သို့) အများကို စွဲ၍ sweep ပြုလုပ်ကာ အထူတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_AdditiveHelix.svg  style="width:32px;"> [Additive helix](PartDesign_AdditiveHelix.md): စကစ်ကို helix တစ်ခုအပြီး sweep ပြုလုပ်ကာ အထူတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_AdditiveBox.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Create an additive primitive:

  -<img alt="" src=images/PartDesign_AdditiveBox.svg  style="width:32px;"> [Additive box](PartDesign_AdditiveBox.md): additive box တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditiveCylinder.svg  style="width:32px;"> [Additive cylinder](PartDesign_AdditiveCylinder.md): additive cylinder တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditiveSphere.svg  style="width:32px;"> [Additive sphere](PartDesign_AdditiveSphere.md): additive sphere တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditiveCone.svg  style="width:32px;"> [Additive cone](PartDesign_AdditiveCone.md): additive cone တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditiveEllipsoid.svg  style="width:32px;"> [Additive ellipsoid](PartDesign_AdditiveEllipsoid.md): additive ellipsoid တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditiveTorus.svg  style="width:32px;"> [Additive torus](PartDesign_AdditiveTorus.md): additive torus တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditivePrism.svg  style="width:32px;"> [Additive prism](PartDesign_AdditivePrism.md): additive prism တစ်ခု ဖန်တီးသည်။

  -<img alt="" src=images/PartDesign_AdditiveWedge.svg  style="width:32px;"> [Additive wedge](PartDesign_AdditiveWedge.md): additive wedge တစ်ခု ဖန်တီးသည်။

#### ဖြုတ်ပစ် ကိရိယာများ (Subtractive tools)

ဤကိရိယာများသည် ရှိပြီးသား Body မှ ပစ္စည်းကို ဖြုတ်ပစ်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/PartDesign_Pocket.svg  style="width:32px;"> [Pocket](PartDesign_Pocket.md): ရွေးချယ်ထားသော စကစ်မှ pocket တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_Hole.svg  style="width:32px;"> [Hole](PartDesign_Hole.md): ရွေးချယ်ထားသော စကစ်မှ ဖြုတ်ပစ်ရန် hole feature တစ်ခု ဖန်တီးသည်။ စကစ်တွင် အဝိုင်းတစ်ခုသို့မဟုတ် အများရှိရမည်။

-   <img alt="" src=images/PartDesign_Groove.svg  style="width:32px;"> [Groove](PartDesign_Groove.md): စကစ်ကို အက်ဆစ်တစ်ခုအပေါ် လှည့်ပတ်၍ groove တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_SubtractiveLoft.svg  style="width:32px;"> [Subtractive loft](PartDesign_SubtractiveLoft.md): နှစ်ခု သို့မဟုတ် ထို့ထက်ပိုသော စကစ်များအကြား ပြောင်းလဲမှုတစ်ခုဖြင့် အထူပုံစံ တစ်ခု ဖန်တီးပြီး လက်ရှိ body ထဲမှ ဖြုတ်ပစ်သည်။

-   <img alt="" src=images/PartDesign_SubtractivePipe.svg  style="width:32px;"> [Subtractive pipe](PartDesign_SubtractivePipe.md): ဖလှယ်ပတ်လမ်းတစ်ခုအပေါ် စကစ်များကို sweep ပြုလုပ်ကာ အထူပုံစံတစ်ခု ဖန်တီးပြီး လက်ရှိ body မှ ဖြုတ်ပစ်သည်။

-   <img alt="" src=images/PartDesign_SubtractiveHelix.svg  style="width:32px;"> [Subtractive helix](PartDesign_SubtractiveHelix.md): စကစ်ကို helix ပေါ် sweep ပြုလုပ်ကာ အထူပုံစံတစ်ခု ဖန်တီးပြီး လက်ရှိ body မှ ဖြုတ်ပစ်သည်။

-   <img alt="" src=images/PartDesign_SubtractiveBox.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Create a subtractive primitive:

  -<img alt="" src=images/PartDesign_SubtractiveBox.svg  style="width:32px;"> [Subtractive box](PartDesign_SubtractiveBox.md): လက်ရှိ body ထဲသို့ subtractive box တစ်ခု အသုံးပြု၍ ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractiveCylinder.svg  style="width:32px;"> [Subtractive cylinder](PartDesign_SubtractiveCylinder.md): လက်ရှိ body ထဲသို့ subtractive cylinder တစ်ခု ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractiveSphere.svg  style="width:32px;"> [Subtractive sphere](PartDesign_SubtractiveSphere.md): လက်ရှိ body ထဲသို့ subtractive sphere တစ်ခု ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractiveCone.svg  style="width:32px;"> [Subtractive cone](PartDesign_SubtractiveCone.md): လက်ရှိ body ထဲသို့ subtractive cone တစ်ခု ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractiveEllipsoid.svg  style="width:32px;"> [Subtractive ellipsoid](PartDesign_SubtractiveEllipsoid.md): လက်ရှိ body ထဲသို့ subtractive ellipsoid တစ်ခု ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractiveTorus.svg  style="width:32px;"> [Subtractive torus](PartDesign_SubtractiveTorus.md): လက်ရှိ body ထဲသို့ subtractive torus တစ်ခု ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractivePrism.svg  style="width:32px;"> [Subtractive prism](PartDesign_SubtractivePrism.md): လက်ရှိ body ထဲသို့ subtractive prism တစ်ခု ထည့်သွင်းသည်။

  -<img alt="" src=images/PartDesign_SubtractiveWedge.svg  style="width:32px;"> ‎[Subtractive wedge](PartDesign_SubtractiveWedge.md): လက်ရှိ body ထဲသို့ subtractive wedge တစ်ခု ထည့်သွင်းသည်။

#### Boolean

-   <img alt="" src=images/PartDesign_Boolean.svg  style="width:32px;"> [Boolean operation](PartDesign_Boolean.md): တစ်ခု သို့မဟုတ် အများသော Bodies သို့မဟုတ် PartDesign Clones များကို လက်ရှိ body ထဲသို့ import လုပ်ကာ Boolean လုပ်ဆောင်ချက် အမျိုးအစားကို သုံးပြီး အလုပ်လုပ်သည်။

### အလှဆင် ကိရိယာများ (Dress-up tools)

ဤကိရိယာများသည် အနွံ (edges) သို့မဟုတ် မျက်နှာပြင် (faces) များကို ကုသမှုတစ်ခုခု လုပ်ပေးသည်။

-   <img alt="" src=images/PartDesign_Fillet.svg  style="width:32px;"> [Fillet](PartDesign_Fillet.md): လက်ရှိ body ၏ အနွံများကို fillet (round) ပြုလုပ်သည်။

-   <img alt="" src=images/PartDesign_Chamfer.svg  style="width:32px;"> [Chamfer](PartDesign_Chamfer.md): လက်ရှိ body ၏ အနွံများကို chamfer ပြုလုပ်သည်။

-   <img alt="" src=images/PartDesign_Draft.svg  style="width:32px;"> [Draft](PartDesign_Draft.md): လက်ရှိ body ၏ ရွေးချယ်ထားသော မျက်နှာပြင်များပေါ် သတ်မှတ်ထားသော ထောင့်ဆ (angular) draft ကို ချရေးပေးသည်။

-   <img alt="" src=images/PartDesign_Thickness.svg  style="width:32px;"> [Thickness](PartDesign_Thickness.md): လက်ရှိ body ထံမှ အထူရှိသော shell တစ်ခု ဖန်တီးကာ ရွေးထားသော မျက်နှာပြင်ကို ဖွင့်ထားပေးသည်။

### ပြောင်းလဲခြင်း ကိရိယာများ (Transformation tools)

ဤကိရိယာများသည် ရှိပြီးသား feature များကို ပြောင်းလဲရန် အသုံးပြုသည်။

-   <img alt="" src=images/PartDesign_Mirrored.svg  style="width:32px;"> [Mirrored](PartDesign_Mirrored.md): feature တစ်ခု သို့မဟုတ် အများကို မျှတကူးယူ (mirror) ပြုလုပ်သည်။

-   <img alt="" src=images/PartDesign_LinearPattern.svg  style="width:32px;"> [Linear Pattern](PartDesign_LinearPattern.md): feature တစ်ခု သို့မဟုတ် အများ၏ တန်းလိုက် အကြိမ်ပြန် pattern တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_PolarPattern.svg  style="width:32px;"> [Polar Pattern](PartDesign_PolarPattern.md): feature တစ်ခု သို့မဟုတ် အများ၏ ဝိုင်းပတ် အကြိမ်ပြန် pattern တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_MultiTransform.svg  style="width:32px;"> [Create MultiTransform](PartDesign_MultiTransform.md): အထက်ဖော်ပြထားသည့် ပြောင်းလဲမှုများနှင့် [Scaled](PartDesign_Scaled.md) ပြောင်းလဲမှုကို ပေါင်းစပ်၍ pattern တစ်ခု ဖန်တီးသည်။
    -   <img alt="" src=images/PartDesign_Scaled.svg  style="width:32px;"> [Scaled](PartDesign_Scaled.md): feature တစ်ခု သို့မဟုတ် အများကို ပမာဏချဲ့ထွင်တိုးချဲ့ (scale) ပြုလုပ်သည်။ ၎င်းသည် သီးခြား ပြောင်းလဲမှု ကိရိယာအဖြစ် မရရှိနိုင်ပါ။

#### ထပ်ဆောင်းများ (Extras)

Part Design မီနူးတွင် တွေ့ရှိရနိုင်သည့် ထပ်ဆောင်း လုပ်ဆောင်ချက်များအချို့။

-   <img alt="" src=images/PartDesign_Sprocket.svg  style="width:32px;"> [Sprocket](PartDesign_Sprocket.md): padded လုပ်နိုင်သည့် sprocket profile တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_InvoluteGear.svg  style="width:32px;"> [Involute gear](PartDesign_InvoluteGear.md): padded လုပ်နိုင်သည့် involute gear profile တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/PartDesign_WizardShaft.svg  style="width:32px;"> [Shaft design wizard](PartDesign_WizardShaft.md): တန်ဖိုးဇယားတစ်ခုအား အခြေခံ၍ shaft တစ်ခု ထုတ်လုပ်ပေးပြီး အာနိသင်နှင့် ကိုက်ကွက်အား (forces and moments) ကို ခွဲခြမ်းစိတ်ဖြာစစ်ဆေးနိုင်စေသည်။ Shaft သည် တည်းဖြတ်နိုင်သည့် revolved sketch ဖြင့် ပြုလုပ်ထားသည်။

### Context Menu အချက်များ 

-   [Suppressed](PartDesign_Suppressed.md): သတ်မှတ်ထားသော feature ကို ဖျက်မထားဘဲ မလည်ပတ်အောင် ပိတ်ထားရန် checkbox။ <small>(v1.0)</small> 

-   <img alt="" src=images/PartDesign_MoveTip.svg  style="width:32px;"> [Set tip](PartDesign_MoveTip.md): Body အပြင်ပိုင်း၌ ဖော်ပြထားသော feature ကို ပြန်သတ်မှတ်ရန် tip ကို ပြင်ဆင်သည်။

-   <img alt="" src=images/PartDesign_MoveFeature.svg  style="width:32px;"> [Move object to other body](PartDesign_MoveFeature.md): ရွေးထားသော စကစ်၊ datum ဂျီအိုမက်ထရီ သို့မဟုတ် feature ကို အခြား Body သို့ ရွှေ့ရာ၌ အသုံးပြုသည်။

-   <img alt="" src=images/PartDesign_MoveFeatureInTree.svg  style="width:32px;"> [Move object after other object](PartDesign_MoveFeatureInTree.md): Body tree ကို ပြန်စီမံရန် ရွေးထားသော စကစ်၊ datum ဂျီအိုမက်ထရီ သို့မဟုတ် feature ကို ကိုယ်လိုချင်သည့် အနေအထားသို့ ရွှေ့ယူနိုင်သည်။

#### Part workbench နှင့် မျှဝေသုံးစွဲသော အချက်များ 

-   <img alt="" src=images/Std_SetAppearance.svg  style="width:32px;"> [Appearance](Std_SetAppearance.md): တစ်ခုလုံး၏ ပြပွားမှု (အရောင်၊ မျက်နှာကြည်ခြင်းစသည်) ကို သတ်မှတ်သည်။

-   <img alt="" src=images/Part_ColorPerFace.svg  style="width:32px;"> [Color per face](Part_ColorPerFace.md): အရာဝတ္ထုတစ်ခုလုံး၏ မျက်နှာပြင် တစ်ခုချင်းစီအား အရောင် သတ်မှတ်ပေးသည်။

### အသုံးမရှိတော့သော ကိရိယာများ (Obsolete tools)

-   <img alt="" src=images/PartDesign_Migrate.svg  style="width:32px;"> [Migrate](PartDesign_Migrate.md): FreeCAD 0.17 မပြည့်မီ ဗားရှင်းများမှ 0.17 သို့ ဖိုင်များကို မိုင်ဂရိတ် ပြုလုပ်သည်။ ဤကိရိယာသည် <small>(v1.0)</small> တွင် မရရှိနိုင်တော့ပါ။

## ဦးစားပေး သတ်မှတ်ချက်များ (Preferences)

-   <img alt="" src=images/Preferences-part_design.svg  style="width:32px;"> [Preferences](PartDesign_Preferences.md): PartDesign ကိရိယာများအတွက် ရရှိနိုင်သည့် preferences များ။
-   [Fine tuning](Fine-tuning.md): PartDesign အပြုအမူကို ပိုမိုနည်းကျစွာ ညှိနှိုင်းရန် ထပ်ဆောင်း ပါရာမီတာများ။

## သင်ခန်းစာများ (Tutorials)

-   [How to use FreeCAD](http://help-freecad-jpg87.fr/), မက်ကနစ် ဒီဇိုင်း အလုပ်စဉ်နှင့် ပတ်သက်သော workflow ကို ရှင်းလင်းဖော်ပြထားသော ဝဘ်ဆိုက်။
-   [Creating a simple part with PartDesign](Creating_a_simple_part_with_PartDesign.md)
-   [Basic Part Design Tutorial 019](Basic_Part_Design_Tutorial_019.md)
-   [PartDesign Bearingholder Tutorial I](PartDesign_Bearingholder_Tutorial_I.md) (needs updating)
-   [PartDesign Bearingholder Tutorial II](PartDesign_Bearingholder_Tutorial_II.md) (needs updating)

## ဥပမာများ (Examples)

Part Design ကိရိယာများဖြင့် ဆောင်ရွက်နိုင်သော အရာများအကြောင်း အနည်းငယ် အကြံဉာဏ် ရရှိရန် [PartDesign examples](PartDesign_Examples.md) ကို ကြည့်ပါ။

 <img alt="" src=images/PartDesign_ExampleSphere-02.png  style="width:80px;"> <img alt="" src=images/PartDesign_ExampleTorus-01.png  style="width:80px;"> <img alt="" src=images/PartDesign_ExamplePad-09.png  style="width:80px;"> <img alt="" src=images/PartDesign_ExampleSweep-02.png  style="width:80px;"> <img alt="" src=images/PartDesign_ExampleSweep-05.png  style="width:80px;"> <img alt="" src=images/PartDesign_ExampleSpring-04.png  style="width:80px;">



---
⏵ [documentation index](../README.md) > [Workbenches](Category_Workbenches.md) > [PartDesign](Category_PartDesign.md) > အစိတ်အပိုင်း ဒီဇိုင်း လုပ်ငန်းခွင် (PartDesign Workbench)