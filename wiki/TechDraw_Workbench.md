## နိဒါန်း (Introduction)

<img alt="" src=images/Workbench_TechDraw.svg  style="width:24px;"> [TechDraw Workbench (နည်းပညာဆိုင်ရာ ပုံဆွဲခြင်း လုပ်ငန်းခွင်)](TechDraw_Workbench.md) ကို [Part](Part_Workbench.md)၊ [PartDesign](PartDesign_Workbench.md) သို့မဟုတ် [BIM](BIM_Workbench.md) ကဲ့သို့သော အခြားလုပ်ငန်းခွင်များဖြင့် ဖန်တီးထားသော သို့မဟုတ် အခြားအက်ပလီကေးရှင်းများမှ တင်သွင်းထားသော ၃ဘက်မြင် မော်ဒယ်များမှ အခြေခံ နည်းပညာဆိုင်ရာ ပုံဆွဲချက်များ (technical drawings) ကို ထုတ်လုပ်ရန် အသုံးပြုသည်။ ပုံဆွဲချက်တစ်ခုစီသည် စာမျက်နှာ (Page) တစ်ခုဖြစ်ပြီး၊ ၎င်းတွင် Part::Features၊ PartDesign::Bodies၊ App::Part အုပ်စုများနှင့် စာတမ်းအရာဝတ္ထု (Document Object) အုပ်စုများကဲ့သို့သော ပုံဆွဲနိုင်သည့် အရာဝတ္ထုများ၏ အမျိုးမျိုးသော မြင်ကွင်းများ (Views) ပါဝင်နိုင်သည်။ ရရှိလာသော ပုံဆွဲချက်များကို မှတ်တမ်းပြုစုခြင်း၊ ထုတ်လုပ်မှုဆိုင်ရာ ညွှန်ကြားချက်များ၊ စာချုပ်များ၊ ခွင့်ပြုမိန့်များ စသည်တို့အတွက် အသုံးပြုနိုင်သည်။

တိုင်းတာချက်များ (Dimensions)၊ ဖြတ်ပိုင်းများ (sections)၊ မျဉ်းစောင်းခြယ် ဧရိယာများ (hatched areas)၊ မှတ်ချက်များ (annotations) နှင့် [SVG](SVG.md) သင်္ကေတများကို စာမျက်နှာတွင် ထည့်သွင်းနိုင်ပြီး၊ ၎င်းတို့ကို [DXF](DXF.md)၊ [SVG](SVG.md) နှင့် [PDF](PDF.md) ကဲ့သို့သော ပုံစံအမျိုးမျိုးဖြင့် ထပ်မံတင်ပို့ (export) နိုင်သည်။

အကယ်၍ သင်၏ အဓိကရည်မှန်းချက်မှာ ရှုပ်ထွေးသော ၂ဘက်မြင် (2D) ပုံဆွဲချက်များနှင့် [DXF](DXF.md) ဖိုင်များ ထုတ်လုပ်ရန်ဖြစ်ပြီး ၃ဘက်မြင် (3D) မော်ဒယ်လ်ပြုလုပ်ရန် မလိုအပ်ပါက ဖရီးကက် (FreeCAD) သည် သင့်အတွက် မှန်ကန်သော ရွေးချယ်မှု မဟုတ်နိုင်ပါ။ ထိုအစား [LibreCAD](https://en.wikipedia.org/wiki/LibreCAD) သို့မဟုတ် [QCad](https://en.wikipedia.org/wiki/QCad) ကဲ့သို့သော နည်းပညာဆိုင်ရာ ပုံဆွဲခြင်းအတွက် သီးသန့်ထုတ်လုပ်ထားသည့် ဆော့ဖ်ဝဲလ်ပရိုဂရမ်တစ်ခုကို အသုံးပြုရန် စဉ်းစားသင့်ပါသည်။

<img alt="" src=images/TechDraw_Workbench_Example.png  style="width:600px;">

## Snapping (စွဲကပ်ခြင်း)

<small>(v1.0)</small> 

: TechDraw Workbench တွင် snapping (စွဲကပ်ခြင်း) အင်္ဂါရပ် ပါရှိသည်။ ၎င်းကို မြင်ကွင်းများ၊ ဖြတ်ပိုင်းမြင်ကွင်းများနှင့် တိုင်းတာချက်များကို မောက်စ်ဖြင့် ဆွဲရွှေ့၍ နေရာချရာတွင် အလိုအလျောက် ချိန်ညှိရန် အသုံးပြုနိုင်သည်။ [ဦးစားပေး သတ်မှတ်ချက်များ (preferences)](TechDraw_Preferences#Snapping.md) တွင် **Snap View Alignment** ကို ဖွင့်ထားပါက (စံနှုန်းအတိုင်း) မြင်ကွင်းများသည် အခြားမြင်ကွင်းများနှင့် လုံလောက်စွာ နီးကပ်သောအခါ ချိန်ညှိမှုဖြစ်စေရန် စွဲကပ်သွားမည်ဖြစ်သည် (**View Snapping Factor** သတ်မှတ်ချက်)။ တိုင်းတာချက်များသည်လည်း အခြားပြိုင်တိုင်းတာချက်များနှင့် စွဲကပ်သွားပြီး တိုင်းတာချက်စာသားကို တိုင်းတာချက်မျဉ်း၏ အလယ်ဗဟိုတွင် စွဲကပ်စေနိုင်သည်။ **Alt** ခလုတ်ကို ဖိထားခြင်းဖြင့် snapping ကို ယာယီပိတ်ထားနိုင်သည်။

## ကိရိယာများ (Tools)

### စာမျက်နှာများ (Pages)

-   <img alt="" src=images/TechDraw_PageDefault.svg  style="width:32px;"> [Insert Default Page (စံစာမျက်နှာ ထည့်သွင်းရန်)](TechDraw_PageDefault.md): စံနှုန်းမီ [နမူနာပုံစံ (template)](TechDraw_Templates.md) ကို အသုံးပြု၍ စာမျက်နှာအသစ်တစ်ခု ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_PageTemplate.svg  style="width:32px;"> [Insert Page using Template (နမူနာပုံစံ အသုံးပြု၍ စာမျက်နှာ ထည့်သွင်းရန်)](TechDraw_PageTemplate.md): ရွေးချယ်ထားသော [နမူနာပုံစံ (template)](TechDraw_Templates.md) ကို အသုံးပြု၍ စာမျက်နှာအသစ်တစ်ခု ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_FillTemplateFields.svg  style="width:32px;"> [Update template fields (နမူနာပုံစံ ကွက်လပ်များကို အပ်ဒိတ်လုပ်ရန်)](TechDraw_FillTemplateFields.md): <small>(v1.0)</small> 

-   <img alt="" src=images/TechDraw_RedrawPage.svg  style="width:32px;"> [Redraw Page (စာမျက်နှာကို ပြန်လည်ဆွဲရန်)](TechDraw_RedrawPage.md): ရွေးချယ်ထားသော စာမျက်နှာကို အပ်ဒိတ်ဖြစ်စေရန် အတင်းအကျပ် လုပ်ဆောင်သည်။

-   <img alt="" src=images/TechDraw_PrintAll.svg  style="width:32px;"> [Print All Pages (စာမျက်နှာအားလုံးကို ပရင့်ထုတ်ရန်)](TechDraw_PrintAll.md): စာတမ်းအတွင်းရှိ စာမျက်နှာအားလုံးကို ပရင့်ထုတ်သည်။ <small>(v0.21)</small> 

-   <img alt="" src=images/TechDraw_ExportPageSVG.svg  style="width:32px;"> [Export Page as SVG (စာမျက်နှာကို SVG အဖြစ် တင်ပို့ရန်)](TechDraw_ExportPageSVG.md): လက်ရှိစာမျက်နှာကို [SVG](SVG.md) ဖိုင်အဖြစ် သိမ်းဆည်းသည်။

-   <img alt="" src=images/TechDraw_ExportPageDXF.svg  style="width:32px;"> [Export Page as DXF (စာမျက်နှာကို DXF အဖြစ် တင်ပို့ရန်)](TechDraw_ExportPageDXF.md): လက်ရှိစာမျက်နှာကို [DXF](DXF.md) ဖိုင်အဖြစ် သိမ်းဆည်းသည်။

### မြင်ကွင်းများ (Views)

#### TechDraw မြင်ကွင်းများ 

-   <img alt="" src=images/TechDraw_View.svg  style="width:32px;"> [Insert View (မြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_View.md): အရာဝတ္ထုတစ်ခု သို့မဟုတ် တစ်ခုထက်ပိုသော အရာဝတ္ထုများ၏ ကိုယ်စားပြုမှုကို ထည့်သွင်းသည်။ <small>(v1.0)</small> : ၎င်းသည် မြင်ကွင်းတစ်ခုတည်း၊ [Projection Group](TechDraw_ProjectionGroup.md)၊ [Spreadsheet View](TechDraw_SpreadsheetView.md)၊ [Arch View](TechDraw_ArchView.md)၊ [Symbol (သင်္ကေတ)](TechDraw_Symbol.md) သို့မဟုတ် [Image View (ပုံရိပ် မြင်ကွင်း)](TechDraw_Image.md) တို့ကို ဖန်တီးနိုင်သည်။

-   <img alt="" src=images/TechDraw_BrokenView.svg  style="width:32px;"> [Insert Broken View (ဖြတ်တောက်ထားသော မြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_BrokenView.md): အရာဝတ္ထုတစ်ခု သို့မဟုတ် တစ်ခုထက်ပိုသော အရာဝတ္ထုများ၏ ဖြတ်တောက်ထားသော မြင်ကွင်းကို ထည့်သွင်းသည်။ <small>(v1.0)</small> 

-   <img alt="" src=images/TechDraw_SectionView.svg  style="width:32px;"> [Insert Section View (ဖြတ်ပိုင်း မြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_SectionView.md): လက်ရှိရှိနေသော မြင်ကွင်းတစ်ခု၏ ကန့်လန့်ဖြတ် ဖြတ်ပိုင်းမြင်ကွင်းကို ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_ComplexSection.svg  style="width:32px;"> [Insert Complex Section View (ရှုပ်ထွေးသော ဖြတ်ပိုင်း မြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_ComplexSection.md): ပရိုဖိုင်တစ်ခုပေါ်တွင် အခြေခံ၍ လက်ရှိရှိနေသော မြင်ကွင်းတစ်ခု၏ ကန့်လန့်ဖြတ် ဖြတ်ပိုင်းမြင်ကွင်းကို ထည့်သွင်းသည်။ <small>(v0.21)</small> 

-   <img alt="" src=images/TechDraw_DetailView.svg  style="width:32px;"> [Insert Detail View (အသေးစိတ် မြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_DetailView.md): လက်ရှိရှိနေသော မြင်ကွင်းတစ်ခု၏ အစိတ်အပိုင်းတစ်ခုကို အသေးစိတ်မြင်ကွင်းအဖြစ် ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_ProjectionGroup.svg  style="width:32px;"> [Insert Projection Group (ပရိုဂျက်ရှင် အုပ်စု ထည့်သွင်းရန်)](TechDraw_ProjectionGroup.md): အရာဝတ္ထုတစ်ခု၏ မတူညီသော လမ်းကြောင်းများမှ မြင်ကွင်းအမျိုးမျိုးကို ဖန်တီးရန် ဒိုင်ယာလော့ဂ်တစ်ခုကို ခေါ်ယူသည်။ <small>(v1.0)</small> : [Insert View](TechDraw_View.md) ကိရိယာကို ထိုအစား အသုံးပြုနိုင်သည်။

-   <img alt="" src=images/TechDraw_ClipGroup.svg  style="width:32px;"> [Insert Clip Group (ကလစ် အုပ်စု ထည့်သွင်းရန်)](TechDraw_ClipGroup.md): ကလစ် အုပ်စုတစ်ခုကို ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_Symbol.svg  style="width:32px;"> [Insert SVG Symbol (SVG သင်္ကေတ ထည့်သွင်းရန်)](TechDraw_Symbol.md): [SVG](SVG.md) ဖိုင်တစ်ခုမှ သင်္ကေတကို စာမျက်နှာအတွင်းသို့ ထည့်သွင်းသည်။ <small>(v1.0)</small> : [Insert View](TechDraw_View.md) ကိရိယာကို ထိုအစား အသုံးပြုနိုင်သည်။

-   <img alt="" src=images/TechDraw_Image.svg  style="width:32px;"> [Insert Bitmap Image (ဘစ်မက်ပ် ပုံရိပ် ထည့်သွင်းရန်)](TechDraw_Image.md): PNG သို့မဟုတ် JPG [ဘစ်မက်ပ် (bitmap)](bitmap.md) ပုံရိပ်ကို စာမျက်နှာအတွင်းသို့ ထည့်သွင်းသည်။ <small>(v1.0)</small> : [Insert View](TechDraw_View.md) ကိရိယာကို ထိုအစား အသုံးပြုနိုင်သည်။

-   <img alt="" src=images/TechDraw_ShareView.svg  style="width:32px;"> [Share View (မြင်ကွင်း မျှဝေရန်)](TechDraw_ShareView.md): စာမျက်နှာအမျိုးမျိုးအကြား မြင်ကွင်းတစ်ခုကို မျှဝေအသုံးပြုသည်။

-   <img alt="" src=images/TechDraw_ToggleFrame.svg  style="width:32px;"> [Turn View Frames On/Off (မြင်ကွင်းဘောင်များ ဖွင့်/ပိတ်ရန်)](TechDraw_ToggleFrame.md): မြင်ကွင်းကို ဝန်းရံထားသော ဘောင်များနှင့် အညွှန်းများကို ဖွင့်/ပိတ် ပြုလုပ်သည်။

-   <img alt="" src=images/TechDraw_ProjectShape.svg  style="width:32px;"> [Project Shape (ပုံသဏ္ဌာန် ပရိုဂျက်လုပ်ရန်)](TechDraw_ProjectShape.md): [3D view (၃ဘက်မြင် အမြင်)](3D_view.md) ရှိ ပုံသဏ္ဌာန်များ၏ ပရိုဂျက်ရှင်များကို ဖန်တီးသည်။

#### အခြားလုပ်ငန်းခွင်များမှ မြင်ကွင်းများ 

-   <img alt="" src=images/TechDraw_ActiveView.svg  style="width:32px;"> [Insert Active View (လက်ရှိမြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_ActiveView.md): တက်ကြွနေသော ၃ဘက်မြင် မြင်ကွင်းကို ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_DraftView.svg  style="width:32px;"> [Insert Draft Workbench Object (ဒရပ်ဖ် လုပ်ငန်းခွင် အရာဝတ္ထု ထည့်သွင်းရန်)](TechDraw_DraftView.md): [Draft Workbench (ဒရပ်ဖ် လုပ်ငန်းခွင်)](Draft_Workbench.md) အရာဝတ္ထုတစ်ခု၏ မြင်ကွင်းကို ထည့်သွင်းသည်။

-   <img alt="" src=images/TechDraw_ArchView.svg  style="width:32px;"> [Insert BIM Workbench Object (BIM လုပ်ငန်းခွင် အရာဝတ္ထု ထည့်သွင်းရန်)](TechDraw_ArchView.md): [BIM Workbench](BIM_Workbench.md) ၏ [Arch Section Plane (အာ့ခ် ဖြတ်ပိုင်း မျက်နှာပြင်)](Arch_SectionPlane.md) အရာဝတ္ထုတစ်ခု၏ မြင်ကွင်းကို ထည့်သွင်းသည်။ <small>(v1.0)</small> : [Insert View](TechDraw_View.md) ကိရိယာကို ထိုအစား အသုံးပြုနိုင်သည်။

-   <img alt="" src=images/TechDraw_SpreadsheetView.svg  style="width:32px;"> [Insert Spreadsheet View (တွက်ချက်မှုဇယား မြင်ကွင်း ထည့်သွင်းရန်)](TechDraw_SpreadsheetView.md): [Spreadsheet Workbench (တွက်ချက်မှုဇယား လုပ်ငန်းခွင်)](Spreadsheet_Workbench.md) ဇယားတစ်ခု၏ မြင်ကွင်းကို ထည့်သွင်းသည်။ <small>(v1.0)</small> : [Insert View](TechDraw_View.md) ကိရိယာကို ထိုအစား အသုံးပြုနိုင်သည်။

### Stacking (အစီအစဉ်ချခြင်း)

ဤအရာများသည် စာမျက်နှာပေါ်ရှိ မြင်ကွင်းများ၏ အနက် (depth) ကို ထိန်းချုပ်ရန်အတွက် အစီအစဉ်ပြောင်းလဲပေးသည့် ကိရိယာများ ဖြစ်သည်။

-   <img alt="" src=images/TechDraw_StackTop.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Adjust Stacking Order (အစီအစဉ်ကို ချိန်ညှိရန်):

  - <img alt="" src=images/TechDraw_StackTop.svg  style="width:32px;"> [Move view to top of stack (အပေါ်ဆုံးသို့ ရွှေ့ရန်)](TechDraw_StackTop.md): မြင်ကွင်းများကို အစီအစဉ်၏ အပေါ်ဆုံးသို့ ရွှေ့သည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/TechDraw_StackBottom.svg  style="width:32px;"> [Move view to bottom of stack (အောက်ဆုံးသို့ ရွှေ့ရန်)](TechDraw_StackBottom.md): မြင်ကွင်းများကို အစီအစဉ်၏ အောက်ဆုံးသို့ ရွှေ့သည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/TechDraw_StackUp.svg  style="width:32px;"> [Move view up one level (တစ်ဆင့်အပေါ်သို့ ရွှေ့ရန်)](TechDraw_StackUp.md): မြင်ကွင်းများကို အစီအစဉ်တွင် တစ်ဆင့်အပေါ်သို့ ရွှေ့သည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/TechDraw_StackDown.svg  style="width:32px;"> [Move view down one level (တစ်ဆင့်အောက်သို့ ရွှေ့ရန်)](TechDraw_StackDown.md): မြင်ကွင်းများကို အစီအစဉ်တွင် တစ်ဆင့်အောက်သို့ ရွှေ့သည်။ <small>(v0.21)</small> 

### Dimensions (တိုင်းတာချက်များ)

-   <img alt="" src=images/TechDraw_Dimension.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Dimensions (တိုင်းတာချက်များ):

  - <img alt="" src=images/TechDraw_Dimension.svg  style="width:32px;"> [Insert Dimension (တိုင်းတာချက် ထည့်သွင်းရန်)](TechDraw_Dimension.md): ဆက်စပ်မှုရှိသော တိုင်းတာချက်တစ်ခုကို ထည့်သွင်းသည်။ <small>(v1.0)</small> 

  - <img alt="" src=images/TechDraw_LengthDimension.svg  style="width:32px;"> [Insert Length Dimension (အလျား တိုင်းတာချက် ထည့်သွင်းရန်)](TechDraw_LengthDimension.md): အလျား တိုင်းတာချက်တစ်ခု ထည့်သွင်းသည်။

  - <img alt="" src=images/TechDraw_HorizontalDimension.svg  style="width:32px;"> [Insert Horizontal Dimension (အလျားလိုက် တိုင်းတာချက် ထည့်သွင်းရန်)](TechDraw_HorizontalDimension.md): အလျားလိုက် အလျား တိုင်းတာချက်တစ်ခု ထည့်သွင်းသည်။
