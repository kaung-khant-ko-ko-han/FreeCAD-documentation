## နိဒါန်း (Introduction)

ပုံရိပ်ဖော်ထုတ်ခြင်း လုပ်ငန်းခွင် (Render Workbench) သည် အိုးပင်းဆော့စ် ပြင်ပ ပုံရိပ်ဖော် အင်ဂျင်များ (external rendering engines) ကို အသုံးပြု၍ ဖရီးကက် (FreeCAD) မော်ဒယ်များမှ အရည်အသွေးမြင့် ပုံရိပ်များကို ထုတ်လုပ်ရန် ခွင့်ပြုသည်။

Image:Pabellon_de_Barcelona.png\|ဘာစီလိုနာ ပွဲကြည့်ဆောင် (Barcelona pavilion)
Screenshot Image:Pabellon_de_Barcelona_Pov_large.png\|ဘာစီလိုနာ ပွဲကြည့်ဆောင်
Povray rendering Image:Pabellon_de_Barcelona_Cycles.png\|ဘာစီလိုနာ ပွဲကြည့်ဆောင်
Cycles rendering Image:Asm_V4.png\|Asm V4
Screenshot Image:Asm_V4_lux.png\|Asm V4
LuxCore rendering Image:Asm_V4_ospray2.png\|Asm V4
Ospray rendering Image:Church_of_the_light.png\|အလင်းဘုရားကျောင်း (Church of the light)
Screenshot Image:Church_of_the_light_lux2.png\|အလင်းဘုရားကျောင်း
LuxCore rendering Image:Church_of_the_light_cycles.png\|အလင်းဘုရားကျောင်း
Cycles rendering Image:Car.png\|ကား
Screenshot Image:Car_ospray.png\|ကား
Ospray rendering Image:Car_lux.png\|ကား
LuxCore rendering Image:Brick_assembly.png\|အုတ်စီခြင်း အစုအဝေး (Brick assembly)
Screenshot Image:Brick_assembly_appleseed.png\|အုတ်စီခြင်း အစုအဝေး
Appleseed rendering Image:Brick_assembly_luxcore.png\|အုတ်စီခြင်း အစုအဝေး
Luxcore rendering Image:VillaSavoye.png\|ဗီလာဆာဗွိုင်း (Villa Savoye)
Screenshot Image:VillaSavoye appleseed.png\|ဗီလာဆာဗွိုင်း
Appleseed rendering Image:VillaSavoye Cycles.png\|ဗီလာဆာဗွိုင်း
Cycles rendering

ပိုင်သွန် (Python) သီးသန့်ဖြင့် ရေးသားထားသော လုပ်ငန်းခွင်ဖြစ်ပြီး၊ Render သည် ဖရီးကက်တွင် အဆင်ပြေချောမွေ့စွာ ပေါင်းစပ်ထားပါသည် - အရာဝတ္ထုများ၊ အလင်းအမှောင်၊ ပစ္စည်းများ (materials)၊ ကင်မရာ စသည့် ပုံရိပ်ဖော် မြင်ကွင်းတစ်ခုလုံးကို ဖရီးကက် အရာဝတ္ထုများဖြင့် ဖော်ပြနိုင်ပြီး ပြင်ပ ပုံရိပ်ဖော်စနစ်များသို့ တင်ပို့ (export) နိုင်ပါသည်။

အခြားသော တတိယပါတီ ကွန်ပျူတာဂရပ်ဖစ် အက်ပလီကေးရှင်းများအပေါ် အခြေခံသည့် နည်းလမ်းများနှင့် နှိုင်းယှဉ်ပါက Render သည် အောက်ပါတို့ကို ရည်ရွယ်ပါသည် -

-   အသုံးပြုသူအနေဖြင့် အခြားသော ၃ဘက်မြင်/ကွန်ပျူတာ ဂရပ်ဖစ် ဆော့ဖ်ဝဲလ်များကို ထပ်မံလေ့လာရန် မလိုအပ်စေရန် - သင်သိလိုသမျှသည် ဖရီးကက်တွင်သာ ရှိပါသည်။
-   ပုံရိပ်ဖော်ခြင်း လုပ်ငန်းစဉ်ကို ရိုးရှင်းစေရန်နှင့် အသုံးပြုသူအား တင်သွင်းခြင်း၊ တင်ပို့ခြင်း၊ မြင်ကွင်း ပြင်ဆင်ခြင်း စသည့် ကြားခံဖိုင် ကိုင်တွယ်မှုများမှ သက်သာစေရန်။
-   မြင်ကွင်း ပြင်ဆင်မှုများကို အမြဲတမ်း တည်ရှိနေစေရန် (persistent) ပြုလုပ်ပေးပြီး၊ အထူးသဖြင့် မော်ဒယ်ကို ပြင်ဆင်လိုက်တိုင်း ပြင်ပကိရိယာတစ်ခုတွင် ထပ်ခါတလဲလဲ ပြန်လည်ပြင်ဆင်ရခြင်းမှ ကာကွယ်ရန်။

## ထောက်ပံ့ပေးထားသော ပုံရိပ်ဖော်စနစ်များ (Supported renderers)

လက်ရှိတွင် ပုံရိပ်ဖော် အင်ဂျင် ခြောက်မျိုးကို ထောက်ပံ့ပေးထားပါသည် -

-   LuxCoreRender
-   Appleseed
-   Cycles (သီးသန့်ဗားရှင်း)
-   Pov-Ray
-   Intel Ospray Studio
-   Pbrt-v4 (စမ်းသပ်အဆင့်)

## အသုံးပြုပုံ (Usage)

အမြန်စတင်ခြင်း (quick-start) စနစ်တွင်၊ လုပ်ငန်းခွင်ကို မှန်ကန်စွာ တပ်ဆင်ပြီးနောက် ဖရီးကက် မော်ဒယ်တစ်ခုကို ပုံရိပ်ဖော်ခြင်းသည် အဆင့် ၄ ဆင့်သာ ရှိပါသည် -

1.  **ပုံရိပ်ဖော် ပရောဂျက်တစ်ခု ဖန်တီးပါ (Create a rendering project):** သင်အသုံးပြုမည့် ပုံရိပ်ဖော်စနစ်နှင့် ကိုက်ညီသော ကိရိယာဘားရှိ ခလုတ်ကို နှိပ်ပြီး သင့်လျော်သော နမူနာပုံစံ (template) ကို ရွေးချယ်ပါ (ဥပမာ - **appleseed_studio_light.appleseed**, **cycles_studio_light.xml**, **luxcore_studio_light.cfg**, **povray_studio_light.pov** စသည်ဖြင့် စတင်နိုင်ပါသည်)။
2.  **သင့်အရာဝတ္ထုများ၏ မြင်ကွင်းများကို ပရောဂျက်ထဲသို့ ထည့်သွင်းပါ (Add views of your objects to your rendering project):** အရာဝတ္ထုများနှင့် ပရောဂျက် နှစ်ခုလုံးကို ရွေးချယ်ပြီး **Add view** ခလုတ်ကို နှိပ်ပါ။
3.  **မြင်ကွင်းကို သတ်မှတ်ပါ (Set your point of view):** [၃ဘက်မြင် မြင်ကွင်းအတွင်း လှည့်လည်ကြည့်ရှုခြင်း (Navigate in the 3D View)](Manual_Navigating_in_the_3D_view.md) ကို အသုံးပြု၍ အလိုရှိသော နေရာသို့ ရွှေ့ပြီး [အမြင်ရှုထောင့် (perspective)](Std_PerspectiveCamera.md) စနစ်သို့ ပြောင်းပါ။
4.  **ပုံရိပ်ဖော်ပါ (Render):** သင့်ပရောဂျက်ကို ရွေးချယ်ပြီး ကိရိယာဘားရှိ **Render** ခလုတ်ကို နှိပ်ပါ (ပရောဂျက်၏ ကွန်တက်မီနူးမှလည်း ရရှိနိုင်ပါသည်)။

**ထိုအခါ သင့်မော်ဒယ်၏ ပထမဆုံး ပုံရိပ်ဖော်ချက်ကို ရရှိမည်ဖြစ်ပါသည်။**

အသေးစိတ် ညွှန်ကြားချက်များကို [GitHub repository](https://github.com/FreeCAD/FreeCAD-render) သို့မဟုတ် အွန်လိုင်း အကူအညီများတွင် ရှာဖွေနိုင်ပါသည်။

## အင်္ဂါရပ်များ (Features)

အင်္ဂါရပ်များတွင် အောက်ပါတို့ ပါဝင်သော်လည်း ၎င်းတို့သာမက အခြားများစွာ ရှိပါသည် -

-   အလင်းအမှောင် (Lighting): အစက်အလင်း (point lights)၊ ဧရိယာအလင်း (area lights)၊ နေနှင့်ကောင်းကင် (sun-sky) နှင့် ကြိုတင်သတ်မှတ်ထားသော အလင်းနမူနာပုံစံများ။
-   ကင်မရာများ (Cameras)။
-   ပစ္စည်းများ စီမံခန့်ခွဲခြင်း (Material management) - (ပုံမှန် shader များဖြစ်သော matte, glossy, glass, principled စသည်တို့ကို အသုံးပြုခြင်း) နှင့် မျက်နှာပြင်များ (textures)။
-   အစုလိုက်လုပ်ဆောင်ခြင်း စနစ် (Batch mode) / UI စနစ်။
-   ဆူညံသံလျှော့ချခြင်း (Denoiser)။
-   ရပ်တန့်ရန် အခြေအနေ (Halt condition)။
-   Meshing ထိန်းချုပ်မှု - ထောင့်ဖြတ်နှင့် မျဉ်းဖြတ် တိမ်းစောင်းမှုများ၊ အလိုအလျောက် ချောမွေ့စေခြင်း (auto-smoothing)။

## လင့်ခ်များ (Links)

ပိုမိုသိရှိလိုပါက: <https://github.com/FreeCAD/FreeCAD-render>

---
⏵ [မှတ်တမ်း အညွှန်း (documentation index)](../README.md) > [ဖြည့်စွက်ချက်များ (Addons)](Category_Addons.md) > [ပြင်ပ အမိန့်ပေးချက်များ ရည်ညွှန်းချက် (External Command Reference)](Category_External%20Command%20Reference.md) > [ပြင်ပ လုပ်ငန်းခွင်များ (External Workbenches)](Category_External%20Workbenches.md) > ပုံရိပ်ဖော်ထုတ်ခြင်း လုပ်ငန်းခွင် (Render Workbench)
