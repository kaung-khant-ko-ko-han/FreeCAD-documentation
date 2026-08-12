**ဗားရှင်း ၀.၂၀ နောက်ပိုင်းတွင် 'Raytracing Workbench' ကို ထည့်သွင်းထားခြင်း မရှိတော့ပါ။<br>
 ပြင်ပ [https://github.com/FreeCAD/FreeCAD-render Render Workbench] ကို အစားထိုး အသုံးပြုသင့်ပါသည်။**

<img alt="Raytracing workbench icon" src=images/Workbench_Raytracing.svg  style="width:128px;">

## နိဒါန်း (Introduction)

<img alt="" src=images/Workbench_Raytracing.svg  style="width:24px;"> [Raytracing Workbench (အလင်းတန်း ခြေရာခံခြင်း လုပ်ငန်းခွင်)](Raytracing_Workbench.md) ကို သင်၏ မော်ဒယ်များကို ပြင်ပ ပုံဖော်စက် (renderer) ဖြင့် လုပ်ဆောင်ခြင်းအားဖြင့် ဓာတ်ပုံကဲ့သို့ အစစ်အမှန်ဆန်သော ပုံရိပ်များ ထုတ်လုပ်ရန် အသုံးပြုသည်။

Raytracing Workbench သည် သင်၏ ၃ဘက်မြင် မော်ဒယ်အတွက် မြင်ကွင်းတစ်ခုကို သတ်မှတ်ပေးသည့် စီမံကိန်းဖိုင်များ ဖြစ်သော [နမူနာပုံစံများ (templates)](Raytracing_templates.md) နှင့် လုပ်ဆောင်သည်။ သင်သည် မီးချောင်းများနှင့် မြေပြင်မျက်နှာပြင်များကဲ့သို့သော ဂျီဩမေတြီများကို ထည့်သွင်းနိုင်ပြီး၊ ၎င်းတွင် ကင်မရာ၏ တည်နေရာနှင့် မြင်ကွင်းအတွင်းရှိ အရာဝတ္ထုများ၏ ပစ္စည်း (material) အချက်အလက်များအတွက် နေရာလွတ်များလည်း ပါဝင်သည်။ ထို့နောက် စီမံကိန်းကို ပုံဖော်ရန် အသင့်ဖြစ်သော ဖိုင်အဖြစ် ထုတ်ယူနိုင်သည် သို့မဟုတ် ဖရီးကက် (FreeCAD) အတွင်း၌ တိုက်ရိုက် ပုံဖော် (render) နိုင်သည်။

လောလောဆယ်တွင် ပုံဖော်စက် (renderers) နှစ်ခုကို ပံ့ပိုးပေးထားသည်: [POV-Ray](POV-Ray.md) နှင့် [LuxRender](LuxRender.md) တို့ ဖြစ်သည်။ ဖရီးကက်အတွင်းမှ ပုံဖော်နိုင်ရန်အတွက် ဤပရိုဂရမ်များအနက် အနည်းဆုံး တစ်ခုကို သင့်စနစ်တွင် တပ်ဆင်ပြီး ပြင်ဆင်ထားရမည်။ သို့သော် ပုံဖော်စက် တစ်ခုမှ တပ်ဆင်မထားပါကလည်း အခြားအချိန်တွင် ပုံဖော်ရန်အတွက် စီမံကိန်းဖိုင်ကို ထုတ်ယူနိုင်ပါသေးသည်။

Raytracing workbench သည် ခေတ်မမီတော့ဘဲ၊ ပြင်ပ [Render Workbench](https://github.com/FreeCAD/FreeCAD-render) သည် ၎င်း၏ အစားထိုးမှု ဖြစ်သည်။ သို့သော်လည်း ဤစာမျက်နှာရှိ အချက်အလက်များသည် လုပ်ငန်းခွင်အသစ်အတွက် ယေဘုယျအားဖြင့် အသုံးဝင်ပါသည်၊ အကြောင်းမှာ နှစ်ခုစလုံးသည် အခြေခံအားဖြင့် တူညီသောနည်းလမ်းဖြင့် လုပ်ဆောင်သောကြောင့် ဖြစ်သည်။

 <img alt="" src=images/Raytracing_example.jpg  style="width:1024px;"> 

## ပုံမှန် လုပ်ငန်းစဉ် (Typical workflow)

၁။ ဖရီးကက် စီမံကိန်းတစ်ခုကို ဖန်တီးပါ သို့မဟုတ် ဖွင့်ပါ၊ အချို့သော  ठोस အရာဝတ္ထုများ ([Part-based](Part_Workbench.md) သို့မဟုတ် [PartDesign-based](PartDesign_Workbench.md)) ကို ထည့်သွင်းပါ; ဇယားကွက်များ (meshes) ကို လောလောဆယ်တွင် ပံ့ပိုးမထားပါ။
၂။ Raytracing စီမံကိန်းတစ်ခု (povray သို့မဟုတ် luxrender) ကို ဖန်တီးပါ။
၃။ Raytracing စီမံကိန်းသို့ သင်ထည့်သွင်းလိုသော အရာဝတ္ထုများကို ရွေးချယ်ပြီး ထည့်သွင်းပါ။
၄။ စီမံကိန်းဖိုင်ကို ထုတ်ယူပါ သို့မဟုတ် ၎င်းကို တိုက်ရိုက် ပုံဖော်ပါ။

<img alt="" src=images/Raytracing_Workbench_workflow.svg  style="width:600px;">

*Raytracing Workbench ၏ လုပ်ငန်းစဉ်; လုပ်ငန်းခွင်သည် ပေးထားသော နမူနာပုံစံမှ စီမံကိန်းဖိုင်တစ်ခုကို ပြင်ဆင်ပြီး၊ မြင်ကွင်း၏ အမှန်တကယ် ပုံဖော်မှုကို ထုတ်လုပ်ရန် ပြင်ပပရိုဂရမ်တစ်ခုကို ခေါ်ယူသည်။ ပြင်ပ ပုံဖော်စက်ကို ဖရီးကက်နှင့် သီးသန့်လွတ်လပ်စွာ အသုံးပြုနိုင်သည်။*

## ကိရိယာများ (Tools)

### စီမံကိန်း ကိရိယာများ (Project tools)

ဤအရာများသည် သင်၏ ၃ဘက်မြင် အလုပ်များကို ပြင်ပ ပုံဖော်စက်များသို့ တင်ပို့ရန်အတွက် အဓိက ကိရိယာများ ဖြစ်သည်။

-   <img alt="" src=images/Raytracing_New.svg  style="width:32px;"> [New PovRay project (PovRay စီမံကိန်းအသစ်)](Raytracing_New.md): စာတမ်းအတွင်း PovRay စီမံကိန်းအသစ် ထည့်သွင်းရန်
-   <img alt="" src=images/Raytracing_Lux.svg  style="width:32px;"> [New LuxRender project (LuxRender စီမံကိန်းအသစ်)](Raytracing_Lux.md): စာတမ်းအတွင်း LuxRender စီမံကိန်းအသစ် ထည့်သွင်းရန်
-   <img alt="" src=images/Raytracing_InsertPart.svg  style="width:32px;"> [Insert part (အစိတ်အပိုင်း ထည့်သွင်းရန်)](Raytracing_InsertPart.md): Raytracing စီမံကိန်းတစ်ခုတွင် အစိတ်အပိုင်းတစ်ခု၏ မြင်ကွင်းကို ထည့်သွင်းရန်
-   <img alt="" src=images/Raytracing_ResetCamera.svg  style="width:32px;"> [Reset camera (ကင်မရာ ပြန်လည်သတ်မှတ်ရန်)](Raytracing_ResetCamera.md): Raytracing စီမံကိန်းတစ်ခု၏ ကင်မရာတည်နေရာကို လက်ရှိမြင်ကွင်းနှင့် ကိုက်ညီအောင် ပြုလုပ်ရန်
-   <img alt="" src=images/Raytracing_ExportProject.svg  style="width:32px;"> [Export project (စီမံကိန်း တင်ပို့ရန်)](Raytracing_ExportProject.md): ပြင်ပ ပုံဖော်စက်တွင် ပုံဖော်ရန်အတွက် Raytracing စီမံကိန်းကို မြင်ကွင်းဖိုင်အဖြစ် တင်ပို့ရန်
-   <img alt="" src=images/Raytracing_Render.svg  style="width:32px;"> [Render (ပုံဖော်ရန်)](Raytracing_Render.md): Raytracing စီမံကိန်းကို ပြင်ပ ပုံဖော်စက်ဖြင့် ပုံဖော်ရန်

### အထောက်အကူပြု ကိရိယာများ (Utilities)

ဤအရာများသည် သီးခြားလုပ်ငန်းဆောင်တာများကို ကိုယ်တိုင်လုပ်ဆောင်ရန် ကူညီပေးသည့် ကိရိယာများ ဖြစ်သည်။

-   <img alt="" src=images/Raytracing_WriteView.svg  style="width:32px;"> [Export view to povray (မြင်ကွင်းကို povray သို့ တင်ပို့ရန်)](Raytracing_WriteView.md): တက်ကြွနေသော ၃ဘက်မြင် မြင်ကွင်းကို ကင်မရာနှင့် ၎င်း၏ ပါဝင်မှုအားလုံးနှင့်အတူ povray ဖိုင်အဖြစ် ရေးသားရန်
-   <img alt="" src=images/Raytracing_WriteCamera.svg  style="width:32px;"> [Export camera to povray (ကင်မရာကို povray သို့ တင်ပို့ရန်)](Raytracing_WriteCamera.md): တက်ကြွနေသော ၃ဘက်မြင် မြင်ကွင်း၏ ကင်မရာတည်နေရာကို POV-Ray ပုံစံဖြင့် ဖိုင်အဖြစ် တင်ပို့ရန်
-   <img alt="" src=images/Raytracing_WritePart.svg  style="width:32px;"> [Export part to povray (အစိတ်အပိုင်းကို povray သို့ တင်ပို့ရန်)](Raytracing_WritePart.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း (အရာဝတ္ထု) ကို povray ဖိုင်အဖြစ် ရေးသားရန်

## ဦးစားပေး သတ်မှတ်ချက်များ (Preferences)

-   <img alt="" src=images/Preferences-raytracing.svg  style="width:32px;"> [Preferences (ဦးစားပေး သတ်မှတ်ချက်များ)](Raytracing_Preferences.md): Raytracing ကိရိယာများအတွက် ရရှိနိုင်သော ဦးစားပေး သတ်မှတ်ချက်များ။
