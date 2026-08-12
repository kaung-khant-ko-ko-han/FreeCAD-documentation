 GuiCommand:
   Name: PartDesign Body
   MenuLocation: Part Design , Create body
   Workbenches: PartDesign_Workbench
   Version: 0.17
   SeeAlso: Std_Part, Feature_editing
---

# အစိတ်အပိုင်း ဒီဇိုင်း ကိုယ်ထည် (PartDesign Body)

## ဖော်ပြချက် (Description)

[PartDesign Body (အစိတ်အပိုင်း ဒီဇိုင်း ကိုယ်ထည်)](PartDesign_Body.md) ဆိုသည်မှာ [PartDesign Workbench (အစိတ်အပိုင်း ဒီဇိုင်း လုပ်ငန်းခွင်)](PartDesign_Workbench.md) ဖြင့်  ठोस ပုံသဏ္ဌာန်များ (solid shapes) ဖန်တီးရန်အတွက် အခြေခံအယ်လ်မင်မစ် ဖြစ်သည်။ ၎င်းတွင် [ပုံကြမ်းများ (sketches)](Sketch.md)၊ [ဒေတမ် အရာဝတ္ထုများ (datum objects)](Datum.md) နှင့် [ဆက်စပ် အင်္ဂါရပ်များ (PartDesign Features)](PartDesign_Feature.md) တို့ ပါဝင်နိုင်ပြီး [တစ်ခုတည်းသော ဆက်စပ်နေသော  ठोस ကိုယ်ထည် (single contiguous solid)](PartDesign_Body#Single_contiguous_solid.md) တစ်ခုကို တည်ဆောက်ရာတွင် အထောက်အကူ ပြုပါသည်။

ဤကိုယ်ထည် (Body) တွင် ဒေသန္တရ X၊ Y နှင့် Z ဝင်ရိုးများအပြင် စံမျက်နှာပြင်များ ပါဝင်သော **Origin** အရာဝတ္ထုတစ်ခု ပါရှိသည်။ ဤအယ်လ်မင်မစ်များကို [ပုံကြမ်းများ (sketches)](Sketch.md) နှင့် [မူလအစ အရာဝတ္ထုများ (primitive objects)](PartDesign_CompPrimitiveAdditive.md) တို့ကို တွဲဆက်ရန်အတွက် ကိုးကားချက်များ (references) အဖြစ် အသုံးပြုနိုင်သည်။

<img alt="" src=images/PartDesign_Body.svg style="width:24px;"> [PartDesign Body](PartDesign_Body.md) ကို <img alt="" src=images/Std_Part.svg style="width:24px;"> [Std Part](Std_Part.md) နှင့် မရောထွေးပါနှင့်။ ပထမတစ်ခုသည် <img alt="" src=images/Workbench_PartDesign.svg style="width:24px;"> [PartDesign Workbench](PartDesign_Workbench.md) တွင် အသုံးပြုသည့် သီးသန့်အရာဝတ္ထုတစ်ခု ဖြစ်ပြီး၊ [PartDesign Features](PartDesign_Feature.md) များ၏ အကူအညီဖြင့် [တစ်ခုတည်းသော ဆက်စပ်နေသော  ठोस ကိုယ်ထည်](PartDesign_Body#Single_contiguous_solid.md) တစ်ခုကို ပုံဖော်ရန် ရည်ရွယ်သည်။ [Std Part](Std_Part.md) သည် [တပ်ဆင်စုစည်းမှုများ (assemblies)](assembly.md) ဖန်တီးရန် ရည်ရွယ်သော အုပ်စုဖွဲ့ အရာဝတ္ထုတစ်ခု ဖြစ်သည်။ ၎င်းကို မော်ဒယ်လ်ပြုလုပ်ရန်အတွက် မဟုတ်ဘဲ အရာဝတ္ထုအမျိုးမျိုးကို အာကာသအတွင်း စီစဉ်ရန်သာ အသုံးပြုသည်။ ရှုပ်ထွေးသော တပ်ဆင်စုစည်းမှုတစ်ခုကို ဖန်တီးရန် ကိုယ်ထည်အများအပြားနှင့် အခြား [Std Parts](Std_Part.md) များကို [Std Part](Std_Part.md) တစ်ခုတည်းအတွင်း၌ ထည့်သွင်းနိုင်ပါသည်။

 ![](images/PartDesign_Body_tree.png ) ![](images/PartDesign_Body_example.png )  
*ဘယ်ဘက်: အရာဝတ္ထု၏ နောက်ဆုံးပုံသဏ္ဌာန်ကို တစ်ခုပြီးတစ်ခု ထုတ်လုပ်ပေးသည့် အင်္ဂါရပ်များကို ပြသနေသော သစ်ပင်ပုံစံ အမြင် (tree view)။ ညာဘက်: [3D view (၃ဘက်မြင် အမြင်)](3D_view.md) တွင် မြင်ရသော နောက်ဆုံးအရာဝတ္ထု။*

## အသုံးပြုပုံ (Usage)

ယခင်က ဖန်တီးထားသော  ठोस ကိုယ်ထည်ကို မရွေးချယ်ထားပါက:

1.  **<img src="images/PartDesign_Body.svg" width=16px> [Body (ကိုယ်ထည်)](PartDesign_Body.md)** ခလုတ်ကို နှိပ်ပါ။ အလွတ်ကိုယ်ထည်တစ်ခု ဖြစ်ပေါ်လာပြီး အလိုအလျောက် **[တက်ကြွသော အခြေအနေ (active)](PartDesign_Body#Active_status.md)** သို့ ရောက်ရှိသွားမည်။
2.  ယခုအခါတွင် **[<img src=images/PartDesign_NewSketch.svg style="width:16px"> [New sketch (ပုံကြမ်းအသစ်)](PartDesign_NewSketch.md)** ကို နှိပ်၍ **[<img src=images/PartDesign_Pad.svg style="width:16px"> [Pad (ပြားချပ်ပိုင်း)](PartDesign_Pad.md)** ဖြင့် အသုံးပြုနိုင်သည့် [ပုံကြမ်း (sketch)](Sketch.md) တစ်ခုကို ကိုယ်ထည်အတွင်း ဖန်တီးနိုင်သည်။
3.  တနည်းအားဖြင့် မူလအစ [PartDesign Feature](PartDesign_Feature.md) တစ်ခုကို ထည့်သွင်းပါ၊ ဥပမာအားဖြင့် **[<img src=images/PartDesign_AdditiveBox.svg style="width:16px"> [Additive box (ထပ်တိုး ဘောက်စ်)](PartDesign_AdditiveBox.md)** ဖြစ်သည်။

 ठोस အရာဝတ္ထုတစ်ခုကို ရွေးချယ်ထားပါက:

1.  **<img src="images/PartDesign_Body.svg" width=16px> [Body (ကိုယ်ထည်)](PartDesign_Body.md)** ခလုတ်ကို နှိပ်ပါ။ တစ်ခုတည်းသော **Base Feature (အခြေခံ အင်္ဂါရပ်)** ပါဝင်သည့် ကိုယ်ထည်အသစ်တစ်ခု ဖြစ်ပေါ်လာမည်။ ဤ Base Feature အယ်လ်မင်မစ်သည် ယခင်က ဖန်တီးခဲ့သော သို့မဟုတ် დုတ္တစာတမ်းအတွင်းသို့ တင်သွင်းခဲ့သော အခြားအရာဝတ္ထုတစ်ခုကို ရိုးရှင်းစွာ ကိုးကားခြင်း ဖြစ်သည်။ ပိုမိုသိရှိလိုပါက [Base Feature](PartDesign_Body#Base_Feature.md) ကို ကြည့်ပါ။ **<img src="images/PartDesign_Body.svg" width=16px> [Body](PartDesign_Body.md)** ကို နှိပ်သည့်အခါ လက်ရှိရှိနေပြီးသား ကိုယ်ထည် သို့မဟုတ် [PartDesign Feature](PartDesign_Feature.md) ကို ရွေးချယ်၍ မရပါ။

### မှတ်ချက်များ (Notes)

-   **[<img src=images/PartDesign_NewSketch.svg style="width:16px"> [New sketch (ပုံကြမ်းအသစ်)](PartDesign_NewSketch.md)** ကို နှိပ်သည့်အချိန်တွင် ကိုယ်ထည် တစ်ခုမှ မရှိသေးပါက ကိုယ်ထည်အသစ်တစ်ခုကို အလိုအလျောက် ဖန်တီးပေးမည်။ ကိုယ်ထည် ရှိပြီးသားဖြစ်ပါက **[<img src=images/PartDesign_NewSketch.svg style="width:16px"> [New sketch](PartDesign_NewSketch.md)** ကို မသုံးမီ ၎င်းကို တက်ကြွအောင် (active) ပြုလုပ်ရမည်။
-   ကိုယ်ထည်ကို တက်ကြွစေရန် သို့မဟုတ် တက်ကြွမှုရပ်ဆဲရန် [tree view (သစ်ပင်ပုံစံ အမြင်)](tree_view.md) ရှိ ကိုယ်ထည်ပေါ်တွင် နှစ်ချက်ကလစ် နှိပ်ပါ (သို့မဟုတ်) ညာဘက်ကလစ်နှိပ်၍ ကွန်တက် မီနူးကို ဖွင့်ကာ **Toggle active body** ကို ရွေးချယ်ပါ။ အခြားကိုယ်ထည်တစ်ခု တက်ကြွနေပါက ၎င်းသည် တက်ကြွမှုရပ်ဆဲသွားမည် ဖြစ်သည်။ ပိုမိုသိရှိလိုပါက [active status (တက်ကြွသော အခြေအနေ)](PartDesign_Body#Active_status.md) ကို ကြည့်ပါ။

## ဂုဏ်သတ္တိများ (Properties)

[PartDesign Body (အစိတ်အပိုင်း ဒီဇိုင်း ကိုယ်ထည်)](PartDesign_Body.md) (`PartDesign::Body` အတန်းအစား) သည် [Part Feature](Part_Feature.md) (`Part::Feature` အတန်းအစား) မှ ဆင်းသက်လာသောကြောင့် နောက်ဆုံးဖော်ပြပါ၏ ဂုဏ်သတ္တိအားလုံးကို ပိုင်ဆိုင်သည်။

[Part Feature](Part_Feature.md) တွင် ဖော်ပြထားသော ဂုဏ်သတ္တိများအပြင် PartDesign Body တွင် [property editor (ဂုဏ်သတ္တိ တည်းဖြတ်ကိရိယာ)](property_editor.md) ၌ အောက်ပါဂုဏ်သတ္တိများ ပါရှိသည်။

### ဒေတာ (Data)

{{TitleProperty|Base}}

-    **Tip|Link**: "Tip" ဟု သတ်မှတ်ထားသော [PartDesign Feature](PartDesign_Feature.md) ဖြစ်ပြီး၊ ပုံမှန်အားဖြင့် ကိုယ်ထည်အတွင်း ဖန်တီးထားသော နောက်ဆုံးအင်္ဂါရပ် ဖြစ်သည်။ Tip သည် ကိုယ်ထည်၏ နောက်ဆုံးပုံသဏ္ဌာန်ကို ညွှန်ပြပြီး၊ **Display Mode Body** ကို `Tip` သို့ သတ်မှတ်ထားသည့်အခါ [3D view (၃ဘက်မြင် အမြင်)](3D_view.md) တွင် ပြသသည်။ ပိုမိုသိရှိလိုပါက [Tip](PartDesign_Body#Tip.md) ကို ကြည့်ပါ။

-    **Base Feature|Link**: ကိုယ်ထည်အတွင်း ပထမဆုံး [PartDesign Feature](PartDesign_Feature.md) အဖြစ် အသုံးပြုသည့် ပြင်ပပုံသဏ္ဌာန် ဖြစ်သည်။ အလွတ်ကိုယ်ထည်တစ်ခုထဲသို့  ठोस အရာဝတ္ထုတစ်ခုကို ဆွဲထည့်သည့်အခါ (drag လုပ်သည့်အခါ) ပုံမှန်အားဖြင့် သတ်မှတ်ပေးသည်။ ဤနည်းလမ်းဖြင့်  ठोस ကိုယ်ထည်ကို မတင်သွင်းရသေးပါက ဤဂုဏ်သတ္တိသည် အလွတ်ဖြစ်နေမည်။ ပိုမိုသိရှိလိုပါက [Base Feature](PartDesign_Body#Base_Feature.md) ကို ကြည့်ပါ။

-    **Placement|Placement**: [3D view (၃ဘက်မြင် အမြင်)](3D_view.md) ရှိ အရာဝတ္ထု၏ တည်နေရာ ဖြစ်သည်။ တည်နေရာကို `Base` အမှတ် (ဗက်တာ) နှင့် `Rotation` (ဝင်ရိုးနှင့် ထောင့်) တို့ဖြင့် သတ်မှတ်သည်။ [Placement](Placement.md) ကို ကြည့်ပါ။

-    **Group|LinkList**: ကိုယ်ထည်အတွင်းရှိ [PartDesign Features](PartDesign_Feature.md) များ ပါဝင်သော စာရင်းတစ်ခု ဖြစ်သည်။
