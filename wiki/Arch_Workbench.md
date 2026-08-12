**ဗားရှင်း ၁.၀ တွင် BIM, Native-IFC နှင့် Arch လုပ်ငန်းခွင်များကို စုစည်းထားသော [BIM လုပ်ငန်းခွင် (BIM Workbench)](BIM_Workbench.md) အဖြစ် ပေါင်းစပ်လိုက်ပြီ ဖြစ်ပါသည်။**

<img alt="Arch workbench icon" src=images/Workbench_Arch.svg  style="width:128px;">

## နိဒါန်း (Introduction)

<img alt="" src=images/Workbench_Arch.svg  style="width:24px;"> [ဗိသုကာဆိုင်ရာ လုပ်ငန်းခွင် (Arch Workbench)](Arch_Workbench.md) သည် ဖရီးကက် (FreeCAD) အတွက် ခေတ်မီသော [**B**uilding **I**nformation **M**odelling](http://en.wikipedia.org/wiki/Building_Information_Modeling) (BIM) လုပ်ငန်းစဉ်ကို ပံ့ပိုးပေးပြီး နံရံများ၊ ထုတ်တန်းများ၊ အမိုးများ၊ ပြတင်းပေါက်များ၊ လှေကားများ၊ ပိုက်လိုင်းများနှင့် ပရိဘောဂများကဲ့သို့သော အပြည့်အဝ ပါရာမက်ထရစ် ဖြစ်သည့် ဗိသုကာဆိုင်ရာ အရာဝတ္ထုများကို ထောက်ပံ့ပေးသည်။ ၎င်းသည် [**I**ndustry **F**oundation **C**lasses](Arch_IFC.md) (IFC) ဖိုင်များကို ထောက်ပံ့ပေးပြီး၊ <img alt="" src=images/Workbench_TechDraw.svg  style="width:24px;"> [TechDraw လုပ်ငန်းခွင် (TechDraw Workbench)](TechDraw_Workbench.md) နှင့် တွဲဖက်၍ ၂ဘက်မြင် အဆောက်အအုံ ပုံစံများ (2D floor plans) ကို ထုတ်လုပ်ပေးနိုင်သည်။

ဗိသုကာဆိုင်ရာ လုပ်ငန်းခွင်သည် ၃ဘက်မြင် ပါရာမက်ထရစ် ဗိသုကာ အရာဝတ္ထုများ တည်ဆောက်ရန် ၎င်း၏ ၂ဘက်မြင် အရာဝတ္ထုများကို အသုံးပြုသောကြောင့် <img alt="" src=images/Workbench_Draft.svg  style="width:24px;"> [ဒရပ်ဖ် လုပ်ငန်းခွင် (Draft Workbench)](Draft_Workbench.md) မှ ကိရိယာအားလုံးကို တင်သွင်းအသုံးပြုသည်။ သို့သော်လည်း Arch သည် <img alt="" src=images/Workbench_Part.svg  style="width:24px;"> [Part](Part_Workbench.md) နှင့် <img alt="" src=images/Workbench_PartDesign.svg  style="width:24px;"> [PartDesign](PartDesign_Workbench.md) ကဲ့သို့သော အခြားလုပ်ငန်းခွင်များဖြင့် ဖန်တီးထားသော solid ပုံသဏ္ဌာန်များကိုလည်း အသုံးပြုနိုင်သည်။

ဖရီးကက်၏ BIM လုပ်ဆောင်ချက်များကို ယခုအခါ အခြေခံ ဗိသုကာဆိုင်ရာ ကိရိယာများပါဝင်သော ဤ Arch လုပ်ငန်းခွင်နှင့် <img alt="" src=images/Std_AddonMgr.svg  style="width:24px;"> [Addon Manager](Std_AddonMgr.md) မှတစ်ဆင့် ရရှိနိုင်သော <img alt="" src=images/Workbench_BIM.svg  style="width:24px;"> [BIM လုပ်ငန်းခွင် (BIM Workbench)](BIM_Workbench.md) ဟူ၍ တဖြည်းဖြည်း ခွဲထုတ်ထားပါသည်။ ဤ BIM လုပ်ငန်းခွင်သည် BIM လုပ်ငန်းစဉ်ကို ပိုမိုလွယ်ကူပြီး အသုံးပြုသူအတွက် အဆင်ပြေစေရန် ရည်ရွယ်၍ Arch ကိရိယာများအပေါ်တွင် interface အလွှာအသစ်တစ်ခု ထပ်မံဖြည့်စွက်ပေးထားသည်။ [FreeCAD BIM ကူးပြောင်းမှု လမ်းညွှန်](https://yorik.uncreated.net/blog/2020-010-freecad-bim-guide) ကို ကြည့်ရှုပါ။

Draft, Arch နှင့် BIM တီထွင်သူများသည် လုံးဝအခမဲ့ ဆော့ဖ်ဝဲလ်များကို အသုံးပြု၍ အဆောက်အအုံ ဒီဇိုင်းများကို မြှင့်တင်ရန် နောက်ဆုံးပန်းတိုင်ဖြင့် ပိုမိုကျယ်ပြန့်သော [OSArch အသိုင်းအဝိုင်း](https://osarch.org) နှင့်လည်း ပူးပေါင်းဆောင်ရွက်လျက် ရှိပါသည်။

 <img alt="" src=images/Screenshot_arch_window.jpg  style="width:600px;"> 

## ကိရိယာများ (Tools)

ဤသည်တို့မှာ ဗိသုကာဆိုင်ရာ အရာဝတ္ထုများ ဖန်တီးရန် ကိရိယာများ ဖြစ်ပါသည်။

-   <img alt="" src=images/Arch_Wall.svg  style="width:32px;"> [နံရံ (Wall)](Arch_Wall.md): အစမှဖြစ်စေ သို့မဟုတ် ရွေးချယ်ထားသော အရာဝတ္ထုတစ်ခုကို အခြေခံ၍ဖြစ်စေ နံရံတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Structure.svg  style="width:32px;"> [တည်ဆောက်ပုံ (Structure)](Arch_Structure.md): အစမှဖြစ်စေ သို့မဟုတ် ရွေးချယ်ထားသော အရာဝတ္ထုတစ်ခုကို အခြေခံ၍ဖြစ်စေ တည်ဆောက်ပုံဆိုင်ရာ အစိတ်အပိုင်းတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_CompRebarStraight.png  style="width:48px;"> [သံချောင်းထည့်သွင်းမှု ကိရိယာများ (Rebar tools)](Arch_CompRebarStraight.md): နောက်ဆုံးတစ်ခုမှလွဲ၍ ဤကိရိယာများကို [Reinforcement လုပ်ငန်းခွင် (Reinforcement Workbench)](Reinforcement_Workbench.md) တပ်ဆင်ထားမှသာ ရရှိနိုင်မည် ဖြစ်သည်။

  - <img alt="" src=images/Reinforcement_StraightRebar.svg  style="width:32px;"> [မျဉ်းဖြောင့် သံချောင်း (Straight Rebar)](Reinforcement_StraightRebar.md): ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း မျဉ်းဖြောင့် သံချောင်းတစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_UShapeRebar.svg  style="width:32px;"> [U-ပုံသဏ္ဌာန် သံချောင်း (U-Shape Rebar)](Reinforcement_UShapeRebar.md): ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း U-ပုံသဏ္ဌာန် သံချောင်းတစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_LShapeRebar.svg  style="width:32px;"> [L-ပုံသဏ္ဌာန် သံချောင်း (L-Shape Rebar)](Reinforcement_LShapeRebar.md): ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း L-ပုံသဏ္ဌာန် သံချောင်းတစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_StirrupRebar.svg  style="width:32px;"> [ကွင်းသံ (Stirrup)](Reinforcement_StirrupRebar.md): ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း ကွင်းသံ (stirrup) တစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_BentShapeRebar.svg  style="width:32px;"> [ကွေးထားသော သံချောင်း (Bent-Shape Rebar)](Reinforcement_BentShapeRebar.md): ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း ကွေးထားသော သံချောင်းတစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_HelicalRebar.svg  style="width:32px;"> [ခရုပတ်ပုံသဏ္ဌာန် သံချောင်း (Helical Rebar)](Reinforcement_HelicalRebar.md): ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း ခရုပတ်ပုံသဏ္ဌာန် သံချောင်းတစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_ColumnRebars.svg  style="width:32px;"> [တိုင် သံချောင်းထည့်သွင်းခြင်း (Column Reinforcement)](Reinforcement_ColumnRebars.md): ရွေးချယ်ထားသော တိုင်အတွင်း သံချောင်းများ ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_BeamRebars.svg  style="width:32px;"> [ထုတ်တန်း သံချောင်းထည့်သွင်းခြင်း (Beam Reinforcement)](Reinforcement_BeamRebars.md): ရွေးချယ်ထားသော ထုတ်တန်းအတွင်း သံချောင်းများ ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_SlabRebars.svg  style="width:32px;"> [ကြမ်းခင်းကွန်ကရစ် သံချောင်းထည့်သွင်းခြင်း (Slab Reinforcement)](Reinforcement_SlabRebars.md): ရွေးချယ်ထားသော ကြမ်းခင်းကွန်ကရစ်အတွင်း သံချောင်းများ ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Reinforcement_FootingRebars.svg  style="width:32px;"> [အုတ်မြစ် သံချောင်းထည့်သွင်းခြင်း (Footing Reinforcement)](Reinforcement_FootingRebars.md): ရွေးချယ်ထားသော အုတ်မြစ်အတွင်း သံချောင်းများ ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Arch_Rebar.svg  style="width:32px;"> [စိတ်ကြိုက် သံချောင်း (Custom Rebar)](Arch_Rebar.md): ပုံကြမ်း (sketch) တစ်ခုကို အသုံးပြု၍ ရွေးချယ်ထားသော တည်ဆောက်ပုံ အစိတ်အပိုင်းတစ်ခုအတွင်း စိတ်ကြိုက် သံချောင်းတစ်ခု ထည့်သွင်းခြင်း။

-   <img alt="" src=images/Arch_CurtainWall.svg  style="width:32px;"> [မှန်ကာရံ (Curtain Wall)](Arch_CurtainWall.md): အစမှဖြစ်စေ သို့မဟုတ် ရွေးချယ်ထားသော အရာဝတ္ထုတစ်ခုကို အခြေခံ၍ဖြစ်စေ မှန်ကာရံတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_BuildingPart.svg  style="width:32px;"> [အဆောက်အအုံ အစိတ်အပိုင်း (Building Part)](Arch_BuildingPart.md): ရွေးချယ်ထားသော အရာဝတ္ထုများ ပါဝင်သည့် အဆောက်အအုံ အစိတ်အပိုင်းတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Project.svg  style="width:32px;"> [စီမံကိန်း (Project)](Arch_Project.md): ရွေးချယ်ထားသော အရာဝတ္ထုများ ပါဝင်သည့် စီမံကိန်းတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Site.svg  style="width:32px;"> [နေရာ (Site)](Arch_Site.md): ရွေးချယ်ထားသော အရာဝတ္ထုများ ပါဝင်သည့် နေရာ (site) တစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Building.svg  style="width:32px;"> [အဆောက်အအုံ (Building)](Arch_Building.md): ရွေးချယ်ထားသော အရာဝတ္ထုများ ပါဝင်သည့် အဆောက်အအုံတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Floor.svg  style="width:32px;"> [အဆင့် (Level)](Arch_Floor.md): ရွေးချယ်ထားသော အရာဝတ္ထုများ ပါဝင်သည့် အထပ်တစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Reference.svg  style="width:32px;"> [ပြင်ပ ရည်ညွှန်းချက် (External reference)](Arch_Reference.md): အခြား ဖရီးကက်ဖိုင်တစ်ခုမှ အရာဝတ္ထုများကို လက်ရှိစာရွက်စာတမ်းအတွင်းသို့ ချိတ်ဆက်ခြင်း။

-   <img alt="" src=images/Arch_Window.svg  style="width:32px;"> [ပြတင်းပေါက် (Window)](Arch_Window.md): အစမှဖြစ်စေ သို့မဟုတ် ရွေးချယ်ထားသော အရာဝတ္ထုတစ်ခုကို အခြေခံ၍ဖြစ်စေ ပြတင်းပေါက်တစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Roof.svg  style="width:32px;"> [အမိုး (Roof)](Arch_Roof.md): ရွေးချယ်ထားသော wire တစ်ခုမှ လျှောစောက်အမိုးတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_CompAxis.png  style="width:48px;"> [ဝင်ရိုး ကိရိယာများ (Axis tools)](Arch_CompAxis.md)

  - <img alt="" src=images/Arch_Axis.svg  style="width:32px;"> [ဝင်ရိုး (Axis)](Arch_Axis.md): တစ်ဘက်သတ် ဝင်ရိုးတန်း (1-direction array of axes) တစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Arch_AxisSystem.svg  style="width:32px;"> [ဝင်ရိုးစနစ် (Axis System)](Arch_AxisSystem.md): ဝင်ရိုးအများအပြားဖြင့် ဖွဲ့စည်းထားသော ဝင်ရိုးစနစ်တစ်ခု ထည့်သွင်းခြင်း။

  - <img alt="" src=images/Arch_Grid.svg  style="width:32px;"> [ဂရစ် (Grid)](Arch_Grid.md): ဂရစ်ပုံစံ အရာဝတ္ထုတစ်ခု ထည့်သွင်းခြင်း။

-   <img alt="" src=images/Arch_SectionPlane.svg  style="width:32px;"> [ဖြတ်ပိုင်းပြင်ညီ (Section Plane)](Arch_SectionPlane.md): ဖြတ်ပိုင်းပြင်ညီ အရာဝတ္ထုတစ်ခု ထည့်သွင်းခြင်း။

-   <img alt="" src=images/Arch_Space.svg  style="width:32px;"> [နေရာလွတ် (Space)](Arch_Space.md): နေရာလွတ် အရာဝတ္ထုတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Stairs.svg  style="width:32px;"> [လှေကား (Stairs)](Arch_Stairs.md): လှေကား အရာဝတ္ထုတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_CompPanel.png  style="width:48px;"> [Panel ကိရိယာများ (Panel tools)](Arch_CompPanel.md)

  - <img alt="" src=images/Arch_Panel.svg  style="width:32px;"> [Panel (Panel)](Arch_Panel.md): ရွေးချယ်ထားသော ၂ဘက်မြင် အရာဝတ္ထုတစ်ခုမှ panel အရာဝတ္ထုတစ်ခု ဖန်တီးခြင်း။

  - <img alt="" src=images/Arch_Panel_Cut.svg  style="width:32px;"> [Panel ဖြတ်ပိုင်း (Panel Cut)](Arch_Panel_Cut.md): panel တစ်ခုမှ ၂ဘက်မြင် ဖြတ်ပိုင်းမြင်ကွင်းတစ်ခု ဖန်တီးခြင်း။

  - <img alt="" src=images/Arch_Panel_Sheet.svg  style="width:32px;"> [Panel စာရွက် (Panel Sheet)](Arch_Panel_Sheet.md): panel ဖြတ်ပိုင်းများ သို့မဟုတ် အခြား ၂ဘက်မြင် အရာဝတ္ထုများ ပါဝင်သော ၂ဘက်မြင် ဖြတ်ပိုင်းစာရွက်တစ်ခု ဖန်တီးခြင်း။

  - <img alt="" src=images/Arch_Nest.svg  style="width:32px;"> [စီစီရီရီ ထည့်သွင်းခြင်း (Nest)](Arch_Nest.md): ပြားချပ်သော အရာဝတ္ထုအများအပြားကို ကွန်တိန်နာ ပုံသဏ္ဌာန်တစ်ခုအတွင်း စီစီရီရီ ထည့်သွင်းခွင့်ပေးခြင်း။

-   <img alt="" src=images/Arch_Equipment.svg  style="width:32px;"> [အသုံးအဆောင်ပစ္စည်း (Equipment)](Arch_Equipment.md): အသုံးအဆောင်ပစ္စည်း သို့မဟုတ် ပရိဘောဂ အရာဝတ္ထုတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Frame.svg  style="width:32px;"> [ဘောင် (Frame)](Arch_Frame.md): ရွေးချယ်ထားသော layout တစ်ခုမှ ဘောင်အရာဝတ္ထုတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Fence.svg  style="width:32px;"> [ခြံစည်းရိုး (Fence)](Arch_Fence.md): ရွေးချယ်ထားသော တိုင်နှင့် လမ်းကြောင်းမှ ခြံစည်းရိုးအရာဝတ္ထုတစ်ခု ဖန်တီးခြင်း။

-   <img alt="" src=images/Arch_Truss.svg  style="width:32px;"> [ထုပ်လျောက် (Truss)](Arch_Truss.md): ရွေးချယ်ထားသော မျဉ်းတစ်ခုမှဖြစ်စေ သို့မဟုတ် အစမှဖြစ်စေ ထုပ်လျောက်တစ်ခု ဖန်တီးခြင်း။

---
⏵ [မှတ်တမ်း အညွှန်း (documentation index)](../README.md) > [လုပ်ငန်းခွင်များ (Workbenches)](Category_Workbenches.md) > [ဗိသုကာ (Arch)](Category_Arch.md) > ဗိသုကာဆိုင်ရာ လုပ်ငန်းခွင် (Arch Workbench)
