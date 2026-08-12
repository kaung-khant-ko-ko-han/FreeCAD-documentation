# <img alt="A2plus workbench icon" src=images/A2p_workbench.svg  style="width:64px;"> A2plus Workbench

## နိဒါန်း

 

A2plus workbench သည် FreeCAD (ဖရီးကက် (FreeCAD)) တွင် မတူညီသည့် အစိတ်အပိုင်းများကို [assemble](Assembly.md) (အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly)) ဖွဲ့စည်းရန် အသုံးပြုသော [external workbench](External_workbenches.md) တစ်ခုဖြစ်သည်။

ဤစာရွက်စာတမ်းသည် A2plus အတွက် ဗားရှင်း **0.4.56 သို့မဟုတ် ပိုမိုသစ်** ဖြစ်သည့် ဗားရှင်းများအတွက် ဖော်ပြထားသည်။

## ထည့်သွင်းခြင်း

A2plus workbench သည် FreeCAD (ဖရီးကက် (FreeCAD)) အတွက် addon တစ်ခုဖြစ်သည်။ ၎င်းကို မူလပလက်ဖောင်းမှ တိုက်ရိုက် ထည့်သွင်းရန် FreeCAD ၏ <img alt="" src=images/AddonManager.svg  style="width:24px;"> [Addon Manager](Std_AddonMgr.md) ကို **Tools → Addon Manager** မီနူး မှတဆင့် အလွယ်တကူ ထည့်သွင်းနိုင်သည်။ A2plus သည် တပ်ဆင်မှုတိုးတက်ရေး ကို ဆက်လက်ဖွံ့ဖြိုးနေသဖြင့် လုပ်ဆောင်ချက်အသစ်များကို မကြာခဏ ထပ်တိုးပေးသည်။ ထို့ကြောင့် သင်သည်လည်း **Tools → [Addon Manager](Std_AddonMgr.md)** မီနူး မှတဆင့် ပုံမှန်နောက်ဆက်တွဲ update လုပ်သင့်သည်။ A2plus ၏ ကုဒ်ကို [GitHub](https://github.com/kbwbe/A2plus) ပေါ်တွင် စီမံထိန်းသိမ်း ဖန်တီး တင်ထားပြီး FreeCAD ၏ **Mod** ဖိုလ်ဒါထဲသို့ မန်ယူးအလိုက် ကော်ပီလုပ်ပြီး လက်လှမ်းမီစွာ လက်ဖြင့် ထည့်သွင်းလည်း ရသည်။

## စတင်အသုံးပြုခြင်း

စတင်ရန် FreeCAD (ဖရီးကက် (FreeCAD)) ထဲတွင် A2plus တူးလ်ဘား သို့ ပြောင်းပါ။ Assembly (အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly)) အသစ်တစ်ခု ဖန်တီးရန် FreeCAD ၌ ဖိုင် အသစ်ဖန်တီးပါ။ အရင်ဆုံး ဤဖိုင်ကို သိမ်းဆည်းရန် လိုအပ်သည်။ သင့်လိုအပ်ချက်အရ (လိုအပ်ပေမယ့် မလိုအပ်ပေ) သင့်တပ်ဆင်လိုသည့် အစိတ်အပိုင်းများရှိသော ဖိုလ်ဒါနှင့် တူညီသော ဖိုလ်ဒါ၌ သိမ်းဆည်းထားသင့်သည်။

ယခု အစိတ်အပိုင်းများကို တူးလ်ဘား ခလုတ် <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> သို့မဟုတ် <img alt="" src=images/A2p_ShapeReference.svg  style="width:24px;"> ကို အသုံးပြု၍ အစီအစဉ်ထဲသို့ ထည့်နိုင်သည်။ <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> ခလုတ်သည် ရွေးထားသော ဖိုင်ရှိ 모든 bodies များကို တစ်ခုတည်းသော part အဖြစ် ထည့်သွင်းသည်။ <img alt="" src=images/A2p_ShapeReference.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပါက ဖိုင်ထဲမှ မည်သည့် part ကို import လုပ်မည်ကို သင့်အား ရွေးချယ်ခွင့် ပေးမည် ဖြစ်သည်။ ဥပမာအားဖြင့် စကစ် (ပုံကြမ်းဖန်တီးမှု (Sketcher)) တစ်ခုသာ import လုပ်ပြီး ထိုစကစ်ကို အသုံးပြု၍ အခြား part များကို တပ်ဆင်ရာတွင် အနေအထား သတ်မှတ်ရန်သာ အသုံးပြုနိုင်သည်။

ပထမတွင် ထည့်သွင်းသော part သည် ပုံမှန်အားဖြင့် fixed position ဖြစ်နေမည်။ (ဤကို နောက်တွင် part property **fixed Position** မှတဆင့် ပြောင်းလဲနိုင်သည်)

Assembly ထဲတွင် ရှိပြီးသား parts များကို <img alt="" src=images/A2p_DuplicatePart.svg  style="width:24px;"> ခလုတ်ဖြင့် ကလုန်း (clone) ပြုလုပ်နိုင်သည်။

Assembly ထဲမှ part တစ်ခုကို တည်းဖြတ်ရန် model tree တွင် ရွေးပြီး <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပါ။ ၎င်းသည် part ဖိုင်ကို FreeCAD ၌ အခြား tab အသစ်တစ်ခုဖြင့် ဖွင့်ပေးမည် သို့မဟုတ် ဖိုင်ကို မကြာခဏ ဖွင့်ထားပြီးသားကိျဗျာဖြစ်လျှင် ၎င်း tab သို့ ပြောင်းလဲပေးမည် ဖြစ်သည်။

Assembly များ၌ ပြောင်းလဲထားသော parts များကို update လုပ်ရန် <img alt="" src=images/A2p_ImportPart_Update.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ။ <img alt="" src=images/A2p_RecursiveUpdate.svg  style="width:24px;"> ခလုတ်သည် parts များကို import လုပ်ပေးသော်လည်း အောက်ပါ [subassemblies](#Subassemblies.md) များကို recursive ဖေါ်ထုတ်ပြီး import လုပ်ပေးပါသည်။ FreeCAD ၏ tree view တွင် part တစ်ခု သို့မဟုတ် အချို့ကို ရွေးထားပါက A2plus သည် ရွေးထားသော part များကို ထောက်ပံ့ update လုပ်ရန် မေးမည် ဖြစ်သည်။

Imported parts များသည် ၎င်းတို့၏ ပြင်ပ အားပံ့ပိုးမှုများကို ထိန်းသိမ်းထားပြီး တည်းဖြတ်နိုင်မည် ဖြစ်သည်။ သို့သော် screws ကဲ့သို့ အကောင်အထည်တည်သော parts များအတွက် ၎င်းတို့၏ shape ကို တည်းဖြတ်၍ မရနေရန် လိုအပ်သည့် အခါများ ရှိသည်။ ၎င်းကို <img alt="" src=images/A2p_ConvertPart.svg  style="width:24px;"> ခလုတ်ဖြင့် ရရှိနိုင်ပြီး ရွေးထားသော part ကို မူရင်း part ၏ static copy အဖြစ် ပြောင်းပေးသည်။

Assembly ကို သိမ်းပြီး ပိတ်လိုလျှင် <img alt="" src=images/A2p_Save_and_exit.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုနိုင်သည်။

<img alt="" src=images/A2p_CD_OneButton.svg  style="width:24px;"> ခလုတ်ကို toggle ပြုလုပ်ခြင်းဖြင့် ရွေးချယ်မှုအမျိုးအစားကို သတ်မှတ်နိုင်သည်။ အထူးသဖြင့် edge, face များကို ရွေးချယ်ရာတွင် တစ်ချက် နှိပ်ခြင်းဖြင့် သို့မဟုတ် **Ctrl**+click ဖြင့် ရွေးချယ်ရန် ရွေးချယ်နိုင်သည်။

## တပ်ဆင်ခြင်း (Assembling)

Parts များကို တပ်ဆင်ခြင်းသည် parts များအကြား ကန့်သတ်ချက် (constraint) များကို ထည့်သွင်းခြင်းဖြင့် ပြုလုပ်သည်။ Constraint တစ်ခု ထည့်သွင်းပြီးနောက် A2plus သည် ၎င်း constraint အရ parts များကို သက်ဆိုင်သလို ရှေ့ဆောင်ပြောင်းလွှတ်ပေးမည် ဖြစ်သည် (ဖြေရှင်းနိုင်ပါက)။

Parts များအကြား constraint တစ်ခု ဖန်တီးရန်အတွက် **Ctrl** key ကို ဖိထားပြီး parts နှစ်ခုစလုံး၏ edge သို့မဟုတ် face တစ်ခုချင်းစီကို ရွေးပါ။ ထို့နောက် သင့်လိုချင်သော constraint ၏ toolbar ခလုတ်ကို နှိပ်ပါ။ ပြတင်းပေါက်တစ်ခု ဖွင့်မည်ဖြစ်ပြီး ၎င်းကို [Constraints](#Constraints.md) အပိုင်းတွင် ဖတ်ရှုနိုင်သည်။ Constraint သည် model tree တွင် သက်ဆိုင်ရာ parts တွင် ဆက်သွယ်ထားသဖြင့် ထည့်သွင်းထားမည် ဖြစ်သည်။

Parts များအကြား ရှုပ်ထွေးသော constraint များကို A2plus သည် တခါတရံ ဖြေရှင်းရန် မအောင်မြင်နိုင်ပါ။ ထို့ကြောင့် ၎င်းအခြေအနေများကို ဖြေရှင်းရာတွင် အကူအညီအဖြစ် [Troubleshooting](#Troubleshooting.md) အပိုင်းကိုလည်း ကြည့်ပါ။

### လိုက်လံကြည့်ရှုခြင်း (Keeping track)

Parts များ အများလာသည့်အခါ နောက်ဆုံးအခြေအနေကို သိရှိထားရမည်မှာ အရေးကြီးလာသည်။ A2plus သည် ထို့အတွက် parts များကို မြှောက်နှိပ်၍ သွားလာပြောင်းလဲရန်နှင့် တွေ့မြင်ရန် အောက်ပါ ကိရိယာများကို ပေးထားသည်။

-   Assembly အတွင်း part တစ်ခုကို တနေရာမှ တနေရာသို့ ဆက်ရွှေ့ရန် model tree တွင် ရွေးပြီး <img alt="" src=images/A2p_MovePart.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပါ။ သင် မိမိထားလိုသည့်နေရာတွင် part ကို တပ်ဆင်ပြီးပါက သက်ဖြင့် လက်ဘက်ကောက်နှိပ်ပါ။ မျှော်လင့်ထားသလို ရွှေ့နေသော part တွင် ရှိပြီးသား constraint များ ရှိလျှင် <img alt="" src=images/A2p_solver.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ခြင်းဖြင့် assembly ၏ အားလုံး constraint များကို ဖြေရှင်းရန် စတင်ပေးမည် ဖြစ်သောကြောင့် ၎င်းအတိုင်း အနေအထားကို ထားပေးမည်။
-   Constraint တစ်ခုကို ပြသရန် model tree တွင် ၎င်းကို ရွေးပြီး <img alt="" src=images/A2p_ViewConnection.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပါ။ ၎င်းသည် အစုံ assembly ကို မျက်နှာပြင် ထိပ်ပြင် ဖျော့ဖျော့ ဖြစ်အောင် ပြသပြီး constraint ဖြင့် ဆက်စပ်ထားသည့် objects နှစ်ခုကို ထူးခြား လှိမ့်ပေးမည်။ ပုံမှန် ကြည့်ရှုမှုသို့ ပြန်သွားရန် assembly အတွင်း ညာဘက်ကလစ် တစ်ချက် နှိပ်ပါ။
-   Assembly ထဲမှ အချို့သော parts များကို သာ ပြသလိုပါက model tree တွင် ထို parts များကို ရွေးပြီး <img alt="" src=images/A2p_Isolate_Element.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပါ။ အခြားနည်းလမ်းတစ်ခုအနေဖြင့် model tree တွင် part တစ်ခုကို ရွေးပြီး **Space** ကို နှိပ်၍ ၎င်း၏ မြင်နိုင်မှုကို toggle ပြုလုပ်၍ ဖျောက်နိုင်သည်။
-   အစုံ assembly ၏ transparency အမြင်ကို toggle ပြုလုပ်ရန် <img alt="" src=images/A2p_ToggleTransparency.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုနိုင်သည်။
-   Part တစ်ခုချင်းစီကို သာမန် FreeCAD (ဖရီးကက် (FreeCAD)) တည်းဖြတ်မှုမှတဆင့် သာမန်အားဖြင့် transparent ပြုလုပ်နိုင်သည်။ သို့သော် အချို့အခါတွင် FreeCAD ၏ bug တစ်ခုကြောင့် assembly ကို ပြန်ဖွင့်သည့်အခါ transparency သတ်မှတ်ချက်များ ပျောက်ဆုံးသွားနိုင်သည်။ workaround အနေဖြင့် <img alt="" src=images/A2p_Restore_Transparency.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြု၍ transparency သတ်မှတ်ချက်များကို ပြန်လည်ထူထောင်နိုင်သည်။

### Constraints

Constraint တစ်ခု ဖန်တီးသောအခါ သင် constraint toolbar ခလုတ်ကို နှိပ်ပြီးနောက် အောက်ပါ ပြတင်းပေါက် ဖြစ်ပေါ်ပြသမည်။

 ![](images/A2p_ConstraintPropertiesDialog.png )  
*အထက်ပါ — A2plus Constraint Properties Dialog*

တချို့သော constraint အမျိုးအစားများအတွက် constraint သဘောတရား၏ ဦးတည်ချက်ကို ပြောင်းလဲနိုင်သည်။ **<img src="images/A2p_solver.svg" width=24px> Solve** ခလုတ်ဖြင့် ဤ constraint အသစ်ကို A2plus ဖြင့် ဖြေရှင်းနိုင်မည့် မဟုတ်မဖြစ်ကို ကြိုစစ်ဆေးနိုင်သည်။ မဖြေရှင်းနိုင်ပါက [Troubleshooting](#Troubleshooting.md) အပိုင်းကို ကြည့်ပါ။

Constraint များကို ၎င်း၏ [visibility](Std_ToggleVisibility.md) ကို ပြောင်းလဲခြင်းဖြင့် ပိတ်ထားနိုင်သည်။ ၎င်းကို tree view တွင် constraint ကို ရွေးပြီး **Space** ကို နှိပ်ခြင်းဖြင့် ပြုလုပ်နိုင်သည်။ ၎င်းသည် **Suppressed** property ကို toggle လုပ်ပေးမည်။ Suppressed ဖြစ်ထားသော constraint တစ်ခုကို assembly ဖြေရှင်းသောအခါ တွက်ချက်ချက်တွင် ထည့်သွင်းမထားပါ။

A2plus သည် အောက်ပါ constraint များကို ပံ့ပိုးပေးသည် — အကြောင်းအရာများကို အသက်သာစေနိုင်ရန် အမျိုးအစားခွဲစိတ်ထားသည်။

#### Point on Point 

Part နှစ်ပိုင်းလုံး၌ [vertex](Glossary#Vertex.md) (point), circle သို့မဟုတ် sphere တစ်ခုကို ရွေးချယ်ပါ။ circle သို့မဟုတ် sphere ကို ရွေးထားခဲ့ပါက ၎င်း၏ center point ကို constraint အတွက် အသုံးပြုမည်။ <img alt="" src=images/A2p_PointIdentity.svg  style="width:24px;"> ခလုတ်သည် {{Variable|pointIdentity}} ဆိုသည့် constraint ကို ထည့်သည်။ ၎င်းသည် vertices များကို coincident ဖြစ်အောင် ပြုလုပ်မည်။

#### Point on Line 

Part တစ်ခုတွင် [vertex](Glossary#Vertex.md) (point) သို့မဟုတ် circular [edge](Glossary#Edge.md) (၎င်း၏ center point ကို ရွေးမည်) သို့မဟုတ် spherical [face](Glossary#Face.md) (၎င်း၏ center point ကိုလည်း ရွေးမည်) တစ်ခုကို ရွေးပြီး အခြား part တွင် [edge](Glossary#Edge.md) တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_PointOnLineConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|pointOnLine}} constraint ကို ထည့်သည်။ ၎င်းသည် vertex ကို edge ပေါ်သို့ တင်ပေးမည်။

#### Point on Plane 

Part တစ်ခုတွင် [vertex](Glossary#Vertex.md) (point) သို့မဟုတ် circular [edge](Glossary#Edge.md) (center point ကို ရွေးမည်) သို့မဟုတ် spherical [face](Glossary#Face.md) (center point ကိုလည်း ရွေးမည်) တစ်ခုကို ရွေးပြီး အခြား part တွင် plane တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_PointOnPlaneConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|pointOnPlane}} constraint ကို ထည့်သည်။ Constraint dialog တွင် point နှင့် plane အကြား offset တစ်ခုကို သတ်မှတ်နိုင်သည်။ ဤ offset ကို plane ၏ နှစ်ဘက်အလှည့်ပြောင်းနိုင်သည်။ offset သည် သုည ဖြစ်လျှင် constraint သည် vertex ကို plane ပေါ်သို့ တင်ပေးမည်။

#### Sphere on Sphere 

Part နှစ်ခုလုံးတွင် spherical [face](Glossary#Face.md) သို့မဟုတ် [vertex](Glossary#Vertex.md) (point) တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_SphericalSurfaceConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|sphereCenterIdent}} constraint ကို ထည့်သည်။ ၎င်းသည် sphere များ၏ center များကို၊ sphere center နှင့် vertex တစ်ခုကို သို့မဟုတ် vertices များကို coincident ဖြစ်အောင် ပြုလုပ်မည်။

#### Circular Edge on Circular Edge 

Part နှစ်ခုလုံးတွင် circular [edge](Glossary#Edge.md) တစ်ခုစီကို ရွေးချယ်ပါ။ <img alt="" src=images/A2p_CircularEdgeConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|circularEdge}} constraint ကို ထည့်သည်။ Constraint dialog တွင် edges များအကြား offset တစ်ခု သတ်မှတ်နိုင်သည်။ ဤ offset ကိုလည်း အလှည့်ပြောင်းနိုင်သည်။ ထို့ပြင် constraint direction သတ်မှတ်ပြီး parts များ၏ rotation ကို lock လုပ်နိုင်သည်။ offset သည် သုည ဖြစ်လျှင် constraint သည် edges များကို 同心円 (concentric) ဖြစ်စေပြီး တူညီသော ပလိန်း(plane) အတွင်းမှာထားမည်။

#### Axis Coincident 

Part နှစ်ခုတွင် cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) တစ်ခုစီကို ရွေးချယ်ပါ။ <img alt="" src=images/A2p_AxialConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|axisCoincident}} constraint ကို ထည့်သည်။ Constraint dialog တွင် axis direction ကို သတ်မှတ်နိုင်သည်။ dialog မှာ parts များ၏ rotation ကို lock လုပ်နိုင်သည့်ရွေးချယ်မှုကိုလည်း ပါဝင်သည်။ ၎င်း constraint သည် axes သို့မဟုတ် lines များကို coincident ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis Parallel 

Part နှစ်ခုတွင် cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) တစ်ခုစီကို ရွေးချယ်ပါ။ <img alt="" src=images/A2p_AxisParallelConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|axisParallel}} constraint ကို ထည့်သည်။ Constraint dialog တွင် axis direction ကို သတ်မှတ်နိုင်သည်။ ၎င်း constraint သည် axes သို့မဟုတ် lines များကို parallel ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis on Plane parallel 

Part တစ်ခုတွင် cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးပြီး အခြား part တွင် plane တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_AxisPlaneParallelConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|axisPlaneParallel}} constraint ကို ထည့်သည်။ ၎င်း constraint သည် axis သို့မဟုတ် line ကို plane နှင့် parallel ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis on Plane normal 

Part တစ်ခုတွင် cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးပြီး အခြား part တွင် plane တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_AxisPlaneNormalConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|axisPlaneNormal}} constraint ကို ထည့်သည်။ ၎င်း constraint သည် axis သို့မဟုတ် line ကို plane အပေါ် မျက်နှာထောင့် (normal) ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis on Plane angle 

Part တစ်ခုတွင် cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးပြီး အခြား part တွင် plane တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_AxisPlaneAngleConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|axisPlaneAngle}} constraint ကို ထည့်သည်။ ၎င်း constraint သည် အရင်ဆုံး axis ကို plane နှင့် parallel ဖြစ်အောင် ပြုလုပ်မည်။ ထို့နောက် constraint settings dialog ထဲတွင် axis အတွက် သတ်မှတ်ထားသော angle ကို ချိန်ညှိနိုင်မည်။

#### Plane Parallel 

Part နှစ်ခုလုံး၌ plane များကို ရွေးပါ။ <img alt="" src=images/A2p_PlanesParallelConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|planesParallel}} constraint ကို ထည့်သည်။ Constraint dialog တွင် constraint direction ကို သတ်မှတ်နိုင်သည်။ ၎င်း constraint သည် plane များကို parallel ဖြစ်အောင် ပြုလုပ်မည်။

#### Plane on Plane 

Part နှစ်ခုလုံး၌ plane များကို ရွေးပါ။ <img alt="" src=images/A2p_PlaneCoincidentConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|planeCoincident}} constraint ကို ထည့်သည်။ Constraint dialog တွင် constraint direction နှင့် plane များအကြား offset တစ်ခုကို သတ်မှတ်နိုင်သည်။ ဤ offset ကိုလည်း အလှည့်ပြောင်းနိုင်သည်။ offset သည် သုည ဖြစ်လျှင် constraint သည် plane များကို coincident ဖြစ်အောင် ပြုလုပ်မည်။

#### Plane Angular 

Part နှစ်ခုလုံး၌ plane များကို ရွေးပါ။ <img alt="" src=images/A2p_AngleConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|angledPlanes}} constraint ကို ထည့်သည်။ Constraint dialog တွင် plane များအကြား angle တစ်ခု သတ်မှတ်နိုင်သည်။ ၎င်း constraint သည် plane များကို အရင်ဆုံး parallel ဖြစ်အောင် ပြုလုပ်ပြီး ထို့နောက် သတ်မှတ်ထားသည့် angle ကို ထပ်သတ်ပေးမည်။

#### Coincidence at Center of Mass 

Part နှစ်ခုလုံး၌ ပိတ်ပင်ထားသော [edge](Glossary#Edge.md) သို့မဟုတ် plane တစ်ခုကို ရွေးပါ။ <img alt="" src=images/A2p_CenterOfMassConstraint.svg  style="width:24px;"> ခလုတ်သည် {{Variable|centerOfMass}} constraint ကို ထည့်သည်။ Constraint dialog တွင် edges သို့မဟုတ် planes များအကြား offset တစ်ခုကို သတ်မှတ်နိုင်သည်။ ဤ offset ကိုလည်း အလှည့်ပြောင်းနိုင်သည်။ ထို့ပြင် constraint direction သတ်မှတ်ခြင်းနှင့် parts များ၏ rotation ကို lock လုပ်နိုင်ပါသည်။ offset သည် သုည ဖြစ်လျှင် constraint သည် edges သို့မဟုတ် planes များကို တူညီသော plane ထဲသို့ တင်ပေးမည်။

### Subassemblies

Assembly တစ်ခုတည်း၌ အခြား assembly များပါဝင်နိုင်သည်။ ၎င်းတို့ကို part များလိုပဲ <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပြီး ***.FCStd** ဖိုင်တစ်ခုကို ရွေးခြင်းဖြင့် ထည့်သွင်းနိုင်သည်။ အမိန့်တန်း subassemblies များကိုလည်း part များလိုပဲ <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ခလုတ်ဖြင့် တည်းဖြတ်နိုင်သည်။ အဆင့်မြင့် assembly များအတွက် တိုးတက်မှုများ ရှိခဲ့ပါက <img alt="" src=images/A2p_RecursiveUpdate.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြု၍ assembly ကို recursive အနေဖြင့် update လုပ်ရန် သေချာစေပါ။

## Constraint Handling 

ရွေးချယ်မှုအတွက် ဖြစ်နိုင်သော constraint များကို toolbar နှင့် *Constraint Tools* dialog တွင် လိုက်ဖော်ပြပါ ခလုတ်များအား ဖွင့်ထားခြင်းဖြင့် ပြသပေးသည်။ *Constraint Tools* dialog ကို <img alt="" src=images/A2p_DefineConstraints.svg  style="width:24px;"> ခလုတ်မှ ဖြင့်လိုက်နိုင်သည်။ ၎င်း dialog သည် ဖွင့်အပ်ထားသည့်အဖြစ် ပြန်ထားရန် ရည်ရွယ်ထားပါသည်၊ ထို့ကြောင့် assembly သို့ constraint များကို အလျင်အမြန် ထည့်သွင်းနိုင်ရန် အဆင်ပြေသည်။

မရှိမဖြစ်ရှိပြီးသား constraints များကို model tree တွင် ရွေးပြီး double-click လုပ်ခြင်း သို့မဟုတ် <img alt="" src=images/A2p_EditConstraint.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုခြင်းဖြင့် တည်းဖြတ်နိုင်သည်။ ၎င်းသည် *Constraint Properties* dialog ကို ဖွင့်ပေးမည်။

Constraint များကို ယာယီ ပိတ်ထားလိုလျှင် model tree တွင် ရွေးပြီး tree element property **Suppressed** ကို ပြောင်းလဲနိုင်သည်။

Constraint များကို ဖျက်ရန် model tree တွင် ရွေးပြီး **Del** ကို နှိပ်ခြင်းဖြင့် သို့မဟုတ် constraints များပါရှိသော part ကို model tree တွင် ရွေးထားပြီး <img alt="" src=images/A2p_DeleteConnections.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြု၍ ဖျက်နိုင်သည်။

Assembly ၏ အားလုံး constraint များကို မည်သည့်အချိန်တွင်မဆို <img alt="" src=images/A2p_solver.svg  style="width:24px;"> ခလုတ်ဖြင့် ဖြေရှင်းနိုင်သည်။ <img alt="" src=images/A2p_ToggleAutoSolve.svg  style="width:24px;"> ခလုတ်ကို ဖွင့်ထားပါက constraint တည်းဖြတ်မှုတိုင်းနောက်တွင် အလိုမလိုက် ဖြေရှင်းသည်။

အစဉ်အလာအရ နောက်ဆုံးထည့်သွင်းထားသော constraint အပေါ်သက်ရောက်မှုကို ပြောင်းလိုပါက <img alt="" src=images/A2p_FlipConstraint.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုနိုင်သည်။ ၎င်းသည် နောက်ဆုံး ထည့်သွင်းထားသော constraint ၏ direction ကို လှေဖျားပြောင်းလဲပေးမည်။

<img alt="" src=images/A2p_CD_ConstraintViewer.svg  style="width:24px;"> ကိရိယာဖြင့် ရှိပြီးသား constraints များကို ပြသ၍ စစ်ဆေးနိုင်သည်။ ၎င်းကို နှိပ်လျှင် dialog တစ်ခု ပေါက်ကာ ပေါ်လာမည်။ ထို့နောက် model tree တွင် part တစ်ခုကို ရွေးပြီး **Import from part** ခလုတ်ကို နှိပ်၍ ထို part ၏ constraint အားလုံးကို ရယူနိုင်သည်။ သို့မဟုတ် tree တွင် constraint များ တစ်ခု သို့မဟုတ် အများကို ရွေးပြီး **Import from Tree** ကို နှိပ်၍ constraint များအကြောင်း အပြည့်အစုံ ရရှိနိုင်သည်။ အားလုံးထဲမှ *Suppress* column တွင် နှိပ်ခြင်းဖြင့် တစ်ခုချင်း constraint ကို suppressed ပြုလုပ်နိုင်သည်။ အခြား dialog ခလုတ်များအတွက် အင်္ဂါရပ်များကို tooltip များမှ ဆက်လက်လေ့လာနိုင်သည်။

## Part Lists

Assembly များအတွက် part list များ ဖန်တီးရန် assembly ၏ အစိတ်အပိုင်းများ အား A2plus မှဖတ်ယူနိုင်သော part info ဖြင့် ဖြည့်ရမည်။ ၎င်းကို part ကို <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ခလုတ်ဖြင့် တည်းဖြတ်ခြင်းမှတဆင့် ပြုလုပ်သည်။ ဖွင့်ထားသော part တွင် <img alt="" src=images/A2p_PartsInfo.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ၊ *#PARTINFO#* ဟု အမည်ရသော [spreadsheet](Spreadsheet_Workbench.md) တစ်ခု ဖန်တီးပေးမည်။

Spreadsheet ၏ ဖွဲ့စည်းပုံမှာ အောက်ပါပုံစံဖြစ်သည်။

![](images/A2p_PartinfoTable.png )

သင့်ထုတ်လွှင့်လိုသော အချက်အလက်များနှင့် ကိုက်ညီသော အမဲ (grey) ရောင်အကွက်များကို ဖြည့်ဆည်းပါ။

Assembly သို့မဟုတ် subassembly တွင် <img alt="" src=images/A2p_PartsList.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပါ။ ၎င်းသည် subassemblies တို့အား အလွှာလိုက် iterate လုပ်လိုသူ မဟုတ်သူ မေးပါလိမ့်မည်။ *Yes* ကို နှိပ်ပါ။ ၎င်းသည် *#PARTSLIST#* ဟု အမည်ပေးထားသော spreadsheet အသစ်ကို ဖန်တီးမည်။ ၎င်းတွင် အပိုင်းများ၏ *#PARTSINFO#* spreadsheets များမှ အချက်အလက်များကို အောက်က ပုံစံအတိုင်း စာရင်းသို့ ထည့်သွင်းပေးမည်။

![](images/A2p_PartslistTable.png )

POS (position) သည် model tree တွင် parts များ ပေါ်လာသည့် အဆင့်အတိုင်း အလိုအလျောက် သတ်မှတ်ပေးသည်။ အထက်ဆုံး အဆင့်ရွိ part သည် POS 1 ကို ရရှိမည်။

QTY (quantity) သည် assembly မှ အလိုအလျောက် တွက်ချက်ပေးသည်။ part တစ်ခုကို assembly တွင် နှစ်ကြိမ် ပါဝင်လျှင် QTY 2 ကို ရမည်။

Part info ကို update ပြုလုပ်ထားပါက <img alt="" src=images/A2p_PartsList.svg  style="width:24px;"> ခလုတ်ကို ထပ်မံ နှိပ်၍ parts list ကို refresh ပြုလုပ်နိုင်သည်။

Subassemblies များအတွက်လည်း <img alt="" src=images/A2p_PartsInfo.svg  style="width:24px;"> ခလုတ်ဖြင့် info spreadsheet တစ်ခု ဖန်တီးနိုင်သည်။ အဓိက assembly ၏ parts list ကို ဖန်တီး သို့မဟုတ် update လုပ်ရာတွင် subassemblies များအား recursive အနေဖြင့် iterate မလုပ်ရန် မေးလျှင် *No* ကို နှိပ်ပါ။ ထိုအချိန်တွင် မူလအားဖြင့် parts များ မပေါ်လာဘဲ subassemblies များသာ parts list ထဲတွင် ပါဝင်မည် ဖြစ်သည်။

## အထူးအင်္ဂါရပ်များ (Special Features)

### Assembly Structure

<img alt="" src=images/A2p_Treeview.svg  style="width:24px;"> ခလုတ်သည် သင့် assembly ၏ ဖွဲ့စည်းပုံ HTML ဖိုင်ကို ဖန်တီးပေးမည်။ ဖိုင်ကို ပုံမှန်အားဖြင့် သင့် assembly ဖိုင်ရှိသော ဖိုလ်ဒါ၌ ထည့်သွင်းမည်။ ဖွဲ့စည်းပုံမှာ အောက်ပါအတိုင်း ဖြစ်သည်။

:   ![](images/A2p_Dependency-Tree.jpg )

### Degrees of Freedom

<img alt="" src=images/A2p_DOFs.svg  style="width:24px;"> ခလုတ်သည် assembly ၏ part တစ်ခုချင်းစီအား ၎င်းတို့၏ degrees of freedom ဖြင့် လုံခြုံအမှတ်တံဆိပ် ချပေးမည်။ ထို့နောက် ၎င်းသည် part များနှင့် ၎င်းတို့၏ dependencies အားလုံးပါသော စာရင်းတစ်ခုကိုထုတ်ပေးမည်။ ၎င်းစာရင်းကို FreeCAD (ဖရီးကက် (FreeCAD)) ၏ *Report view* widget ထဲသို့ ထုတ်ပေးမည်။ ထို widget ကို ယခုအခါ မမြင်နိုင်ဘူးဆိုလျှင် FreeCAD toolbar ဧရိယာ၏ ဖန်အလယ်ပိုင်းကို ညာဘက်ကလစ်နှိပ်၍ ပြသသော context menu ထဲမှ ရွေးချယ်နိုင်သည်၊ သို့မဟုတ် **View → Panels → [Report view](Report_view.md)** မီနူးမှ ဖွင့်နိုင်သည်။

DoF (degrees of freedom) အမှတ်တံဆိပ်များကို ထပ်မံ ဖျက်လိုပါက <img alt="" src=images/A2p_DOFs.svg  style="width:24px;"> ခလုတ်ကို ထပ်မံ နှိပ်ပါ။

### Part Labels

<img alt="" src=images/A2p_PartLabel.svg  style="width:24px;"> ခလုတ်သည် assembly ၏ part တစ်ခုချင်းစီကို 3D view တွင် ၎င်း၏နာမည်ဖြင့် label ထားပေးမည်။ Part labels များကို ဖျက်လိုပါက ထပ်မံ <img alt="" src=images/A2p_PartLabel.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ။

### Shape of whole Assembly

တချို့အချိန်များတွင် assembly အားလုံးကို တစ်ခုထဲသော shape အဖြစ်ပေါင်းစည်းရန် လိုအပ်နိုင်သည်။ ၎င်း shape ကို ဥပမာအားဖြင့် [Mesh workbench](Mesh_Workbench.md) တွင် 3D-printing အတွက် သို့မဟုတ် [TechDraw workbench](TechDraw_Workbench.md) တွင် အပြင်ဆန်းများအတွက် အသုံးပြုနိုင်သည်။ ၎င်းကို <img alt="" src=images/A2p_SimpleAssemblyShape.svg  style="width:24px;"> ခလုတ်ဖြင့် ဖန်တီးနိုင်သည်။ ၎င်း shape ကို မူလအားဖြင့် မမြင်နိုင်အောင်ထားသည်။ Assembly တွင် ပြောင်းလဲမှုများရှိခဲ့ပါက အတူတူသော ခလုတ်နဲ့ shape ကို update ပြုလုပ်နိုင်သည်။

### Convert absolute Paths to relative Ones

မီနူး **A2plus → Misc → [<img src=images/A2p_SetRelativePathes.svg style="width:24px"> Convert absolute paths of imported parts to relative ones]** ကို အသုံးပြု၍ imported parts များ၏ absolute paths များကို relative paths ဖြစ်အောင် ပြောင်းနိုင်သည်။

## Preferences

a2plus preferences များကို FreeCAD (ဖရီးကက် (FreeCAD)) ၏ **Edit → [Preferences](Preferences_Editor.md)** မီနူး ထဲမှ *A2plus* အပိုင်း၌ ဝင်၍ ပြင်ဆင်နိုင်သည်။ အောက်ပါ ရွေးချယ်စရာများကို သတ်မှတ်နိုင်သည်။

### Default solving method

- Use solving of partial systems : solver သည် property **fixed Position** ကို *true* အဖြစ် သတ်မှတ်ထားသော part တစ်ခုနှင့် ၎င်းနှင့် အချက်ပေးထားသော part တစ်ခုနှင့်အတူ စတင်သည်။ အခြား parts များကို မတွက်ချက်ပါ။ အဖြေရှာနိုင်ခဲ့ပါက နောက်ထပ် constrained part တစ်ခုကို တွက်ချက်ချက်ထဲထည့်ပြီး ဆက်လက်လုပ်ဆောင်မည်။
- Use "magnetic" solver, solving all parts at once : solver သည် property **fixed Position** ကို *true* သတ်မှတ်ထားသော part သို့ ဦးတည်ပြီး parts အားလုံးကို တပြိုင်နက်တည်း ဆွဲဆောင်ရန် ကြိုးပမ်းသည်။ ယင်းသည် အများအားဖြင့် ဖြေရှင်းချက် တွက်ချက်ရန် ပိုမိုအချိန်ကုန်စေနိုင်သည်။
- Force fixed position : ဤသည်သည် assembly အတွင်းရှိ parts အားလုံး၏ property **fixed Position** ကို *true* သတ်မှတ်ပေးသည်။ ထို့ကြောင့် parts အားလုံးကို မူလဖန်တီးထားသော မည်သည့်နေရာတွင်မဆို အမြဲတမ်း fixed ဖြစ်နေမည်ဖြစ်၍ တကယ်ထည့်သွင်း၍ တိုင်ပင်ကာ ရှာဖွေမှုကို မလိုအပ်တော့ပါ။

### Default solver behaviour

- Solve automatically if a constraint property is changed : constraint property တစ်ခုကို ပြောင်းလဲသောအခါ solver ကို အလိုအလျောက် စတင်လုပ်ဆောင်မည်။ ၎င်းသည် toolbar အပေါ် <img alt="" src=images/A2p_ToggleAutoSolve.svg  style="width:24px;"> ခလုတ်ကို ဖွင့်ထားသလို ဖြစ်စေသည်။

### Behaviour when updating imported parts

- Recalculate imported parts before updating them : Assembly ၏ အစိတ်အပိုင်းများအားလုံး၊ subassemblies ရောပါပြီး FreeCAD ၌ ဖွင့်၍ spreadsheets များမှ ဂဏန်းများကို အသုံးပြုကာ ပြန်လည်တည်ဆောက်မည်။ ဤအင်္ဂါရပ်သည် စနစ်တကျ ပြီမိုက်စနစ်ဖြင့် ဖန်တီးရန် ရည်ရွယ်ထားသည်။ သတိပြုရန်: ဤအင်္ဂါရပ်သည် အလွန် 실험적 ဖြစ်ပြီး အရေးကြီးသော project များအတွက် မသင့်လျော်ပါ။
  နောက်ဆက်တွဲ ပြဿနာများ -
  - Assembly ကို ဖျက်ပစ်နိုင်သည်၊ အကြောင်းရင်းမှာ parts များ၏ topological names များရှိသော မှားယွင်းသော လင့်ခ်များကြောင့် ဖြစ်သည်။
  - Master spreadsheets များကို အကယ်၍ အမှား ထားပြင်သောအခါ၊ ရည်ညွှန်းထားသော part ဖိုင်ကို ပိတ်ထားသောအချိန်တွင် ပြင်ဆင်လျှင် ဖိုင်များ ပျက်စီးကာ FreeCAD ကို crash ဖြစ်စေနိုင်သည်။

- Enable recursive update of imported parts : subassemblies များအားလုံးကို recursive အတွင်းဖွင့်ခြင်းအားဖြင့် update လုပ်ပေးသည်။

- Use experimental topological naming : parts များကို assembly သို့ import လုပ်စဉ်တွင် algorithm တစ်ခုက subelement တစ်ခုချင်းစီအတွက် topological names များ ထုတ်ပေးသည်။ ထို topological names များကို **mux Info** ထဲသို့ ရေးထည့်သည်။ Imported part တစ်ခု ချိန်ဆင်ရန် လိုအပ်လာသောအခါ၌ ၎င်း topological names များကို သုံးကာ constraints ၏ subelements များကို update ပြုလုပ်နိုင်သည်။ ဒါကြောင့် assembly များသည် FreeCAD ၏ subelement နံပါတ်များ ပြောင်းလဲလှုပ်ရှားမှုဆီမှ ပိုမိုခံနိုင်ရည်ရှိ သွားမည် ဖြစ်သည်။
  သတိပြုရန်: ဤသည်သည် ဖိုင်အရွယ်အစားနှင့် import ဆောင်ရွက်ချိန်တွင် တွက်ချက်ချိန်ကို များစေသည်။ topological naming ကို အသုံးချလိုလျှင် assembly ဖန်တီးမည့် မလုပ်ခင် အဆင့်တွင် ဖွင့်ထားရမည်။

- Inherit per face transparency from parts and subassemblies : imported parts များမှ colour နှင့် transparency setting များကို အလိုအလျောက် သုံးမည်။
  သတိပြုရန်: ဤအင်္ဂါရပ်သည် အလွန် 실험적 ဖြစ်ပြီး အရေးကြီးသော project များအတွက် မသင့်လျော်ပါ။

- Do not import invisible shapes : invisible datum/construction shapes များကို ဖျောက်ပစ်မည်။ သတိပြုရန်: အခြား higher သို့မဟုတ် တခြား subassemblies များတွင် datum/construction shapes များနှင့် constraints များ ဆက်သွယ်ထားမထားသင့်ပါ။ မဟုတ်လျှင် assembly ကို ဖျက်စီးနိုင်သည်။

- Use solid union for importing parts and subassemblies : imported parts များအားလုံးကို တိုက်ရိုက် union အဖြစ် တစ်ခုထဲ ပေါင်းစည်းထားမည်။
  ဤအင်္ဂါရပ်သည် [FEM](FEM_Workbench.md) (Finite Element Method (FEM / အပိုင်းငယ်နည်းစနစ်)) စမ်းသပ်မှုများ သို့မဟုတ် [3D-printing](Manual_Preparing_models_for_3D_printing.md) အတွက် အသုံးဝင်ပါသည်၊ အကယ်၍ တစ်ခုတည်းသော solid သာ ခွင့်ပြုထားရပါက။ အခြားရွေးချယ်စရာမှာ မကြာခဏနောက်ပိုင်းတွင် [shape of the whole assembly](#Shape_of_whole_Assembly.md) ကို ဖန်တီးခြင်း ဖြစ်သည်။

### User interface settings

- Show constraints in toolbar : ဤရွေးချယ်ချက်ကို မသုံးပါက များသော constraint များအတွက် toolbar ခလုတ်များ မမြင်ရတော့ဘဲ toolbar အတွင်း နေရာသိမ်းရန် အတွက် ဖျက်ထားမည်။ အချက် အသစ်များကို *Constraint Tools* dialog (toolbar ခလုတ် <img alt="" src=images/A2p_DefineConstraints.svg  style="width:24px;">) မှတဆင့် ဆက်လက် သတ်မှတ်နိုင်သည်။
- Use native file manager of your OS : ဤ options ကို အသုံးပြုပါက assembly များအတွက် ဖိုင်ရွေးချယ်ရာတွင် သင်၏ OS ၏ native file dialog ကို ရရှိမည်။

### Storage of files

- Use relative paths for imported parts : imported parts များအတွက် relative file paths ကို အသုံးပြုသည်။
- Use absolute paths for imported parts : imported parts များအတွက် absolute file paths ကို အသုံးပြုသည်။
- All files are in this project folder : project ဖိုင်အားလုံးကို သတ်မှတ်ထားသော ဖိုလ်ဒါအတွင်းထားရမည်။ ၎င်းတို့သည် ထိုဖိုလ်ဒါ၏ subfolders များတွင်ရှိပါကလည်း ပြဿနာမရှိ။ သတိပြုရန်: ဖိုင်တစ်ခုကို ဤဖိုလ်ဒါအတွင်း မျိုးချင်းများစွာ (ဥပမာ ဖြင့် မတူညီသော subfolders များ၌) မရှိသင့်ပါ။
  ဤ option သည် မတူညီသော ကွန်ပျူတာပေါ်တွင် အလုပ်လုပ်ရန် အဆင်ပြေစေသည်၊ အကယ်၍ project ဖိုလ်ဒါကို ကူးယူရန်သာ လိုအပ်မည်ဖြစ်သည်။

## ပြဿနာဖြေရှင်းခြင်း (Troubleshooting)

A2plus သည် သင်ထားသော constraints များကို ဖြေရှင်း၍ မရနိုင်သည့် ပြဿနာကို မကြာခဏ တွေ့ကြုံရမည်။ ၎င်းကို ဖြေရှင်းရန် အမျိုးမျိုးသော ဝါလဒ်များရှိသည်။

### Conflict Finder ကိရိယာ အသုံးပြုခြင်း

တူညီသော constraint အများကြားရှိသောအခါ ဤကိရိယာသည် အကောင်းဆုံး နည်းလမ်းဖြစ်သည်၊ အကြောင်းမှာ ဤကိရိယာသည် constraint ကို တစ်ခါတစ်လေစီ ဖြေရှင်းကြည့်၍ ဘာကြောင့် conflict ဖြစ်နေသည်ကို ရှာဖွေပေးနိုင်သည်။ ထိုအခါ တွေ့ရှိထားသော conflicting constraint ကို ဖြေရှင်းရန် အခြား strategy များကို အသုံးပြုနိုင်သည်။ ၎င်းကို <img alt="" src=images/A2p_SearchConstraintConflicts.svg  style="width:24px;"> ခလုတ်ဖြင့် ခေါ်ယူနိုင်သည်။

### Constraint Direction ကို စစ်ဆေးခြင်း

တချို့အခါတွင် constraints များသည် လုံးဝတည်းသလို သတ်မှတ်ထားလည်း သော်လည်း ဖြေရှင်း၍ မရနိုင်စေနိုင်သည်။ ဥပမာ - နှစ်ခုသော plane များအတွက် {{Variable|[planesParallel](#Plane_Parallel.md)}} constraint တစ်ခု ရှိပြီး ယင်း plane များအတွက် {{Variable|[planeCoincident](#Plane_on_Plane.md)}} constraint ကို ထပ်မံ သတ်မှတ်ချင်လျှင် A2plus သည် ဖြေရှင်း၍ မရနိုင်နိုင်သည်။ ဤအချိန်တွင် {{Variable|planesParallel}} နှင့် {{Variable|planeCoincident}} ၏ constraint direction များ ကွာခြားနေခြင်း ဖြစ်နိုင်သည်။ အချိန်တိုင်း၌ နှစ်ခုစလုံးအတွက် အလားတူ direction အသုံးပြုပါ။

A2plus သည် assembly ၏ **အားလုံး** constraint များအတွက် မှန်ကန်သည့် direction ကို အလိုအလျောက် စစ်ဆေးပေးနိုင်သည်။ ၎င်းကို <img alt="" src=images/A2p_ReAdjustConstraints.svg  style="width:24px;"> ခလုတ်ဖြင့် အသုံးပြုနိုင်သည်။

### Constraint များ ဖျက်ခြင်း

ဖြေရှင်း၍ မရသော constraint များအများစုသည် constraint အသစ်တစ်ခု ထည့်သွင်းသည့် ခဏအတွင်း တိုက်ရိုက်ဖြစ်ပေါ်သည်။ ၎င်းအချိန်တွင် ဖြေရှင်းနည်းမှာ နောက်ဆုံးထည့်ထားသော constraint ကို ဖျက်ပစ်ခြင်း ဖြစ်သည်။ A2plus သည် ဤအကြံပြုချက်ကိုလည်း ပေးပါလိမ့်မည်။

တချို့အခါတွင် ဖျက်ခြင်းသာသာ လျှင်သာ ဖြေရှင်းနိုင်သည်၊ ဥပမာ သင်သည် FreeCAD ၌ part တစ်ခုကို တည်းဖြတ်ပြီး constraints နှင့် ဆက်စပ်ထားသော face သို့မဟုတ် edge များ ပျောက်သွားခဲ့လျှင် ဖြစ်နိုင်သည်။ ဤအခါ သင့်လုပ်ရမည့်အချက်မှာ ၎င်း ပြောင်းလဲထားသော part နှင့် ဆက်စပ်နေသော constraint ကို တစ်ချက်ချင်း ဖျက်ပစ်ရမည်ဖြစ်သည်။ ဖျက်ခြင်းတိုင်းနောက် သတ်မှတ်ချက်ကို တွက်ချက်ရန် <img alt="" src=images/A2p_solver.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ။ သင် ဖြေရှင်းနိုင်သည့် အခြေအနေတစ်ခု ရောက်ရှိသည်ကို တွေ့ပါက လိုအပ်သည့် constraint များကို အဆင့်လိုက် ထပ်ထည့်ပါ။

### Parts ကို ရွှေ့တင်ခြင်း (Moving Parts)

တချို့ အခါ၌ solver ၌ သတ်မှတ်ထားသော စတင်တန်ဖိုးများ (start values) ကောင်းမွန်ရန် လိုအပ်သည်။ ဥပမာ အက်စ် (axle) part တစ်ခုနှင့်ဘီး (wheel) part တစ်ခုရှိသည်ဟု ယူပါ။ သင် {{Variable|axisCoincident }} constraint ကို ထည့်သွင်းပြီး solver မှ အချက်မပေးပေမယ့် parts များ မရွှေ့လျှင် FreeCAD ၏ *Report view* တွင် \"*REACHED POS-ACCURACY :0.0*\" ဟူသောစာသားကို မြင်နိုင်သည်။ ဤအခြေအနေတွင် ဖြေရှင်းနည်းတစ်ခုမှာ မည်သည့် parts များကို မျက်နှာချင်းဆိုင်ရောက်အောင် လက်ဖျားဖြင့် နီးစေ့ရွှေ့၍ စတင်တန်ဖိုးများကို ပိုမိုလက်လှမ်းရာချင်း set လုပ်ပေးခြင်း ဖြစ်သည်။

မှတ်ချက်: Constraint ၏ တစ်ခုခုပင်သာ **fixed Position** property ကို *false* သတ်မှတ်ထားရန် သေချာပါစေ။

### Tip Property ကို သတ်မှတ်ခြင်း

Imported part တွင် မျှော်လင့်ထားသည့် အချို့သော feature များ မပေါ်လာခဲ့ပါက property **[Tip](PartDesign_MoveTip.md)** ကို စစ်ဆေးပါ။

A2plus သည် bodies များကို သူတို့တွင် ရှိသည့် features အားလုံးကို tip feature အထိ import လုပ်သည်။ အကြောင်းမှာ tip ကို တစ်ခုချိန်ထားခြင်းသည် tip ထက် ကျော်သန်းသည့် features များကို မမြင်ရစေရန် ရည်ရွယ်မှုဖြစ်သည်။ အကယ်၍ A2plus တွင် part feature တစ်ခု မပေါ်လာခဲ့လျှင် <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ခလုတ်ဖြင့် part ကို ဖွင့်ပြီး body တစ်ခုကို ရွေးပြီး ၎င်း၏ property **Tip** ကို ကြည့်ပါ။ Tip သည် သင်လိုချင်သည့် feature တွင် မရှိပါက လိုချင်သော feature အပေါ် right-click ပြုလုပ်ပြီး **[<img src=images/PartDesign_MoveTip.svg style="width:24px"> Set tip]** ကို ရွေးချယ်ပါ။ နောက်ဆုံးတွင် part ကို သိမ်းပြီး <img alt="" src=images/A2p_ImportPart_Update.svg  style="width:24px;"> ခလုတ်ဖြင့် assembly ကို reload ပြုလုပ်ပါ။

### Assembly Tree ကို ပြင်ဆင်ခြင်း (Repairing Assembly Tree)

Constraint များ မဖြေရှင်းနိုင်သည့် ရှင်းလင်းသော အကြောင်းရင်းကို မမြင်နိုင်ပါက <img alt="" src=images/A2p_RepairTree.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုကြည့်နိုင်သည်။ ၎င်းသည် အားလုံး constraint များကို ဖြေရှင်းပြီး နောက် ပြန်လည် အစိတ်အပိုင်းများအောက်၌ ထပ်မံ အုပ်စုဖွဲ့ပေးမည်။

### အဟောင်း A2plus assemblies များကို မိုင်ဂရိတ် ပြုလုပ်ခြင်း (Migrating old A2plus assemblies)

March 2019 より မတိုင်မီအချိန်တွင် ဖန်တီးထားသော A2plus assemblies များတွင် imported parts အတွက် မှန်ကန်သော icons မပြရန်နှင့် obsolete properties များ ပါဝင်နိုင်သည်။ ဤ assemblies များကို A2plus ဗားရှင်း 0.4.35 နှင့် အထက်သို့ မိုင်ဂရိတ်ပြုလုပ်ရန် **A2plus → Misc → [<img src=images/A2p_Upgrade.svg style="width:24px"> Migrate proxies of imported parts]** မီနူးကို အသုံးပြုပါ။ ပြုလုပ်ခဲ့ပြီးနောက် assembly ဖိုင်ကို သိမ်းပြီး ပြန်ဖွင့်ရပါမည်။

### Accented Characters များ ကင်းရှင်းရန် သတိပေးချက်

**ဤနည်းလမ်းသည် Windows အတွက် မလိုအပ်ပါ။**

အချို့ OS များတွင် part များ သို့မဟုတ် assembly ၏ ဖိုင်နာမည် သို့မဟုတ် ဖိုင်လမ်းကြောင်းများတွင် accent ပါသော character များပါရှိလျှင် ပြဿနာများ ဖြစ်ပေါ်နိုင်သည်။ ထို့ကြောင့် အဲဒီသက်ရောက်မှုရှိသည့် ကာဂျာတွင် accent characters များနှင့် အထူး စာလုံးများကို ရှောင်ကြဉ်ပါ။

### Fixing Position

**ဤနည်းလမ်းသည် A2plus 0.3.11 သို့မဟုတ် ထက်ပိုမိုနောက်သစ်သော assembly များအတွက် မလိုအပ်တော့ပါ၊ အဆိုပါ A2plus အားလုံးသည် ယခု missing fixed positions များအတွက် သတိပေးချက်ထုတ်ပေးသည်။**

သင် parts နှစ်ခုအကြား constraint တင်ရာတွင် မည်သည့် part မှာမဆို property **fixed Position** ကို *true* အဖြစ် သတ်မှတ်ထားခြင်းမရှိပါက သို့မဟုတ် fixed Position = *true* သတ်မှတ်ထားသော part တစ်ခုနှင့် constraint မှတဆင့် ဆက်စပ်ထားသော part မရှိပါက constraint သည် ဖြေရှင်း၍ မရနိုင်ပါ။ ညီမျှသည့် ဖောက်သည်များတွင် ဖိုက်ဆိုလျှင် နှစ်ဖက်စလုံးတွင် **fixed Position** ကို *true* သတ်မှတ်ထားပါကလည်း ထိုအတိုင်း ဖြစ်ပေါ်မည်။

A2plus သည် ဖြေရှင်းမှု မအောင်မြင်ပါက သတင်းအချက်အလက် ထုတ်ပေးမည် ဖြစ်သော်လည်း တခါတရံ သင် သာမန်အားဖြင့် parts များ မရွှေ့ရန်သာ ဖြစ်နိုင်ပြီး FreeCAD ၏ *Report view* widget တွင် \"*REACHED POS-ACCURACY :0.0*\" ဟူသောစာသားကို တွေ့ရနိုင်သည်။ ၎င်းသည် solver သည် အမှားမကျော်ဖြတ်ဘဲပြီးဆုံးသော်လည်း တကယ်တမ်း constraint များကို ဖြေရှင်း၍ မရခြင်းကို အဓိပ္ပါယ်ရသည်။

ထို့ကြောင့် assembly အတွင်းရှိ သင့် part များထဲမှ အနည်းဆုံးတစ်ခုတွင် **fixed Position** ကို *true* သတ်မှတ်ထားခြင်း သေချာစေပါ။ ထို့နောက် သင့်သည် fixed part နှင့် တစ်ဖက်ထဲသို့ ဘယ်လိုမဆို ဆက်နွယ်ထားသော part များကိုသာ constraint များ သတ်မှတ်ပါ။ ၎င်း dependencies များကို မြင်ရန် [Assembly Structure](#Assembly_Structure.md) အပိုင်းကို ကြည့်ပါ။

### Parts ကို လှည့်ခြင်း (Rotating Parts)

**ဤနည်းလမ်းသည် A2plus 0.4.0 သို့မဟုတ် ထက်နောက်သစ်သော assembly များအတွက် မလိုအပ်တော့ပါ၊ A2plus သည် solver အတွက် စတင် angle အထူးတန်ဖိုး ရရှိအောင် နောက်ခံတွင် အနည်းငယ် အလိုအလျောက် rotate ပေးပါသည်။**

solver က {{Variable|angledPlanes}} constraint အတွက် မအောင်မြင်သော အချိန်များ များစွာ ရှိပြီး ၎င်းအကြောင်းရင်းမှာ ရွေးထားသည့် plane နှစ်ခုသည် လောလောဆယ်တွင် 0° သို့မဟုတ် 180° angle ရှိနေခြင်း ဖြစ်နိုင်သည်။ (parts များ မရွှေ့လျှင် FreeCAD ၏ *Report view* တွင် \"*REACHED POS-ACCURACY :0.0*\" ဟူသောစာသားကို မြင်ရမည်။) ၎င်းအတွက် ဖြေရှင်းနည်းမှာ part တစ်ခုကို အချို့ အဆင့်များဖြင့် FreeCAD ၏ transform feature ကို အသုံးပြုကာ (model tree တွင် part ကို right-click → **Transform**) တစ်ဖက်သို့ အနည်းငယ် လှည့်ပေးခြင်း ဖြစ်သည်။

မှတ်ချက်: Constraint ၏ တစ်ပိုင်းဟာ **fixed Position** ကို *false* အဖြစ် သတ်မှတ်ထားရန် သေချာပါစေ။

## အနုပျို ဇာတ်လမ်း (Animation)

A2plus သည် dragging နှင့် Python scripts တို့မှတဆင့် animation များကို ပံ့ပိုးပေးသည်။

### Dragging

Dragging animation များသည် interactive ဖြစ်ပါသည်၊ သင် assembly ၏ part တစ်ခုကို drag လုပ်၍ ထိန်းချုပ်စေနိုင်သည်။ ဤ animation များရရှိရန် -

1.  သာမန် animation များကို ပြုလုပ်လိုသည့် part ကို လုံးဝ constraints ဖြင့် ကန့်သတ်ထားပါ။
2.  <img alt="" src=images/A2p_MovePartUnderConstraints.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ။ ၎င်းသည် dragging mode ကို enable လုပ်မည်။
3.  Assembly ၌ သင့်လိုသည့် part ကို နှိပ်ပါ။
4.  ယခု မောက်စ်ကို လှန်လိုက်သည့်အခါ part သည် သတ်မှတ်ထားသည့် constraints အတွင်း အလျားလိုက် သို့မဟုတ် ခေါင်လိုက် အတိုင်း လှုပ်ရှားသွားမည်။
5.  Dragging mode ကို အဆုံးသတ်ရန် assembly အတွင်း ညာဘက်ကလစ် တစ်ချက်နှိပ်ပါ သို့မဟုတ် ESC ကို နှိပ်ပါ။

Dragging animation ကို လေ့လာရန် example assembly တစ်ခု: [A2p_example-for-dragging-animation.FCStd](https://forum.freecadweb.org/download/file.php?id=99204)

![](images/A2p_dragging-animation-result.gif )

*အထက်ပါ — ဥပမာ assembly ကို အသုံးပြုပြီး dragging animation ကို ပြသခြင်း*

### Scripting

Dragging mode ၌ interactive animations များကို ဖန်တီးနိုင်သော်လည်း screencasts သို့မဟုတ် ဗီဒီယို အတွက် တိကျမှန်ကန်မှု မလုံလောက်နိုင်သဖြင့် scripted animations များကို အသုံးပြုပါက တိကျမှန်ကန်စွာ လှုပ်ရှားမှုများနှင့် လှည့်လျားမှုများကို သတ်မှတ်နိုင်သည်။ ဥပမာ တိကျစွာ 10° ချင်း အနက်အချင်း လှည့်စေလိုပါက scripted animation သည် လွယ်ကူစေမည်။

Scripted animation တစ်ခုသည် ဦးလေးအားဖြင့် အောက်ပါနည်းဖြင့် လည်ပတ်သည် -

1.  Assembly ကို လုံးဝ constraints ဖြင့် ကန့်သတ်ထားသည်။
2.  Script သည် parameter တစ်ခု (ဥပမာ part ၏ position သို့မဟုတ် rotation angle) ကို ပြောင်းသည်။
3.  Parameter ပြောင်းပြီးနောက် assembly constraints များကို ဖြေရှင်းသည်။
4.  အဆင့် 2 နှင့် 3 ကို ထပ်မံလုပ်ဆောင်၍ animation ကို ရရှိစေသည်။

constraint တစ်ခု (ဥပမာ plane နှစ်ခုအကြား distance) ကို အစားထိုးပြောင်းလဲ၍လည်း animation ပြုလုပ်နိုင်သည်။

#### Simple Script Example

အနည်းဆုံးနည်းလမ်းဖြင့် non-interactive animation တစ်ခုကို ရေးနိုင်သည်။ ဥပမာအနေဖြင့် - ဤ assembly ဖိုင်ကို ဒေါင်းလုဒ်လုပ်ပါ: [A2p_animated-example.FCStd](https://forum.freecadweb.org/download/file.php?id=97554) နှင့် Python script ကိုလည်း ဒေါင်းလုဒ်လုပ်ပါ: [A2p_animation-example-script.py](https://forum.freecadweb.org/download/file.php?id=97981)။

<div class="mw-collapsible mw-collapsed toccolours">

 This is the content of the script and the lines beginning with a '#' describe what the different script lines do: 


<div class="mw-collapsible-content">

 
```python
# import libraries
import time, math, PySide
import A2plus.a2p_solversystem as a2p_solver


# we use steps of 1 degree
step = 1
# wait 1 ms between every step
timeout = 0.001
# initial angle is 0 degree
angle = 0
# we take the currently opened document
document = FreeCAD.activeDocument()
# we want later change the rotation angle of the part "star_wheel_001"
starWheel = document.getObject("star_wheel_001")
# define a progress dialog running from 0 to 360
progressDialog = PySide.QtGui.QProgressDialog(u"Animation progress", u"Stop", 0, 360)


# the while block is the main loop to change the angle and solve
# the assembly constraints subsequently
while angle < 360: # run this loop until we have one full turn (360 degrees)
    # increase the rotation angle
    angle += step
    # set the new angle to the progress dialog
    progressDialog.setValue(angle)
    # change the rotation angle of the part "star_wheel_001"
    starWheel.Placement.Rotation.Angle = math.radians(angle)
    # solve the constraints 
    a2p_solver.solveConstraints(document, useTransaction=True)
    # update the view after the solving ('Gui' stands for 'graphical user interface')
    FreeCADGui.updateGui()
    # bring the progress dialog to front
    PySide.QtGui.QWidget.raise_(progressDialog)
    # if 'Stop' was pressed in the dialog, exit the loop
    if progressDialog.wasCanceled():
        angle = 360
    # wait some time before performing the next step
    time.sleep(timeout)
```


</div>


</div>



Script ကို အသုံးပြုပြီး animation ပြုလုပ်ရန် အဆင့်များမှာ -

1.  Assembly ဖိုင်ကို FreeCAD (ဖရီးကက် (FreeCAD)) တွင် ဖွင့်ပါ။
2.  Script ဖိုင်ကို FreeCAD (ဖရီးကက် (FreeCAD)) တွင် ဖွင့်ပါ။
3.  Script (macro) ကို အကောင်အထည်ဖော်ရန် <img alt="" src=images/Menu_Std_DlgMacroExecute_fr_02.png  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ။
4.  Rotation ကို ကြည့်ရန် assembly tab သို့ ပြောင်းပါ။

လေ့ကျင့်ရန် script အတွင်းကို ပြောင်းလဲပြီး ထပ်မံ 실행 ပြုလုပ်ပါ။ ဥပမာတွင် *step* ကို *5* သို့ တိုးလိုက်ပါ။

ဥပမာ animation ၏ ရလဒ်မှာ -

![](images/A2p_animated-example-result.gif )

#### Interactive Script Example

ပထမဥပမာသည် feedback မရှိသည့် non-interactive animation တစ်ခုကို ဖော်ပြခဲ့သည်။ အမြဲတမ်းအများစုလုံးတွင် သင်သည် animation နှင့် အပြန်အလှန် ဆက်ဆံလိုတတ်သည်။ ဥပမာ အထက်ပါ ဥပမာ၌ driving pins များ wheel ၏ center groove ကို ကျော်သွားပတ်သည်ကို မြင်လိုပါက အနီးကပ် ကြည့်ရှုချင်သည်။ ထို့ကြောင့် interactive ဖြေရှင်းချက်တစ်ခု လိုအပ်သည်။

ဒါကို custom animation dialog တစ်ခုနှင့် slider တစ်ခုသုံးကာ ပြုလုပ်နိုင်သည်။ Slider ကို ရွေ့ပြီး rotation angle ကို ပြောင်းလဲနိုင်သည်၊ ထို့ဖြင့် လှည့်ချင်းပြန်ခြင်းနှင့် အတူတူအဆင့်များကို ပြသနိုင်သည်။

အပေါ်ပါ assembly ဖိုင်ထက် အချည်းနှီးသော script ကို အသုံးပြုပါ - [A2p_animated-example.FCStd](https://forum.freecadweb.org/download/file.php?id=97554) နှင့် [A2p_animation-example-script.py](https://forum.freecadweb.org/download/file.php?id=97982)။

<div class="mw-collapsible mw-collapsed toccolours">

 This is the content of the script to get the interactive animation dialog: 


<div class="mw-collapsible-content">

 
```python
# import libraries
import time, math, PySide, sys
import FreeCAD.A2plus.a2p_solversystem as a2p_solver
from FreeCAD import Units
from PySide import QtCore, QtGui


# wait 1 ms after every calculation
timeout = 0.001
# we take the currently opened document
document = FreeCAD.activeDocument()
# we want later change the rotation angle of the part "star_wheel_001"
starWheel = document.getObject("star_wheel_001")


class AnimationDlg(QtGui.QWidget): # the animation dialog

    
def __init__(self): # to initialize the dialog
        super(AnimationDlg, self).__init__()
        self.initUI()

    
def initUI(self): # the definition of the dialog components
        self.setMinimumSize(self.minimumSizeHint()) # set the minimal dialog size to minimum
        self.setWindowTitle('Animation Dialog')
        # use a grid layout for the whole form
        self.mainLayout = QtGui.QGridLayout()
        self.lineNo = 0 # first dialog grid line
        # add description label
        DescriptionLabel = QtGui.QLabel(self)
        DescriptionLabel.setText("Change slider to change rotation angle")
        self.mainLayout.addWidget(DescriptionLabel,self.lineNo,0,1,4)
         # next dialog grid line
        self.lineNo += 1
        # add a label; there is no need for the "self." prefix because we don't want to change the label later
        LabelMin = QtGui.QLabel(self)
        LabelMin.setText("Min")
        LabelMin.setFixedHeight(32)
        self.mainLayout.addWidget(LabelMin,self.lineNo,0)
        # add a spin edit to define the slider minimum
        self.MinEdit = QtGui.QSpinBox(self)
        # get the angle unit as string
        self.MinEdit.setSuffix(" " + str(FreeCAD.Units.Quantity(1, FreeCAD.Units.Angle))[2:])
        self.MinEdit.setMaximum(999)
        self.MinEdit.setMinimum(0)
        self.MinEdit.setSingleStep(10)
        self.MinEdit.setValue(0)
        self.MinEdit.setFixedHeight(32)
        self.MinEdit.setToolTip("Minimal angle for the slider")
        QtCore.QObject.connect(self.MinEdit, QtCore.SIGNAL("valueChanged(int)"), self.setMinEdit)
        self.mainLayout.addWidget(self.MinEdit,self.lineNo,1)
        # add the slider
        self.slider = QtGui.QSlider(QtCore.Qt.Horizontal, self)
        self.slider.setRange(0, 360)
        self.slider.setValue(0)
        self.slider.setFixedHeight(32)
        self.slider.setToolTip("Move the slider to change the rotation angle")
        QtCore.QObject.connect(self.slider, QtCore.SIGNAL("sliderMoved(int)"), self.handleSliderValue)
        self.mainLayout.addWidget(self.slider,self.lineNo,2)
        # add a label
        LabelMax = QtGui.QLabel(self)
        LabelMax.setText("Max")
        LabelMax.setFixedHeight(32)
        self.mainLayout.addWidget(LabelMax,self.lineNo,3)
        # add a spin edit to define the slider maximum
        self.MaxEdit = QtGui.QSpinBox(self)
        # get the angle unit as string
        self.MaxEdit.setSuffix(" " + str(FreeCAD.Units.Quantity(1, FreeCAD.Units.Angle))[2:])
        self.MaxEdit.setMaximum(999)
        self.MaxEdit.setMinimum(1)
        self.MaxEdit.setSingleStep(10)
        self.MaxEdit.setValue(360)
        self.MaxEdit.setFixedHeight(32)
        self.MaxEdit.setToolTip("Maximal angle for the slider")
        QtCore.QObject.connect(self.MaxEdit, QtCore.SIGNAL("valueChanged(int)"), self.setMaxEdit)
        self.mainLayout.addWidget(self.MaxEdit,self.lineNo,4)
         # next dialog grid line
        self.lineNo += 1
        # add a spacer
        self.mainLayout.addItem(QtGui.QSpacerItem(10,10), 0, 0)
        # add a label
        LabelCurrent = QtGui.QLabel(self)
        LabelCurrent.setText("Current angle:")
        LabelCurrent.setFixedHeight(32)
        self.mainLayout.addWidget(LabelCurrent,self.lineNo,1)
        # output the current angle
        self.CurrentAngle = QtGui.QLineEdit(self)
        self.CurrentAngle.setText(str(0))
        self.CurrentAngle.setFixedHeight(32)
        self.CurrentAngle.setToolTip("Current rotation angle")
        self.CurrentAngle.isReadOnly()
        self.mainLayout.addWidget(self.CurrentAngle,self.lineNo,2)
        # add label for the unit
        LabelUnit = QtGui.QLabel(self)
        LabelUnit.setText("deg")
        LabelUnit.setFixedHeight(32)
        self.mainLayout.addWidget(LabelUnit,self.lineNo,3)
        # button to close the dialog
        self.Close = QtGui.QPushButton(self)
        self.Close.setText("Close")
        self.Close.setFixedHeight(32)
        self.Close.setToolTip("Closes the dialog")
        QtCore.QObject.connect(self.Close, QtCore.SIGNAL("clicked()"), self.CloseClicked)
        self.mainLayout.addWidget(self.Close,self.lineNo,4)
        # place the defined grid layout to the dialog
        self.setLayout(self.mainLayout)
        self.update()

    
def handleSliderValue(self):
        # set slider value as angle
        starWheel.Placement.Rotation.Angle = math.radians(self.slider.value())
        # output current angle
        self.CurrentAngle.setText(str(self.slider.value()))
        # solve the constraints 
        a2p_solver.solveConstraints(document)
        # update the view after the solving ('Gui' stands for 'graphical user interface')
        FreeCADGui.updateGui()
        # wait some time, important to give time to perform calculations
        time.sleep(timeout)

    
def setMinEdit(self):
        # assure that the minimum is samller than the maximum
        if self.MinEdit.value() >=  self.MaxEdit.value():
            self.MaxEdit.setValue(self.MinEdit.value() + 1)
        self.slider.setRange(self.MinEdit.value(), self.MaxEdit.value())

    
def setMaxEdit(self):
        # assure that the minimum is samller than the maximum
        if self.MinEdit.value() >=  self.MaxEdit.value():
            self.MinEdit.setValue(self.MaxEdit.value() - 1)
        self.slider.setRange(self.MinEdit.value(), self.MaxEdit.value())

    
def CloseClicked(self):
        AnimationDialog.close()


# create and show the defined dialog
AnimationDialog = AnimationDlg()
AnimationDialog.show()


# run this loop when the dialog is visible
while AnimationDialog.isVisible():
    # update the view; important to give the OS feedback the dialog is alive
    FreeCADGui.updateGui()
    # bring the dialog to front, so that the dialog is always visible
    QtGui.QWidget.raise_(AnimationDialog)
    # output slider value here too because during the calculation the slider might have been moved
    AnimationDialog.CurrentAngle.setText(str(AnimationDialog.slider.value()))
```


</div>


</div>



Script တွင် သတ်မှတ်ထားသည့် dialog သည် အောက်ပါပုံစံရှိသည်။

![](images/A2p_AnimationDialog.png )

### Script Commands

Script syntax ကို ပိုမိုနားလည်ရန် အောက်တွင် အချို့ command များကို ဖော်ပြထားသည်။

အောက်တွင် ဥပမာအားဖြင့် placement property `Rotation.Angle` ကို မိမိ starWheel အဖြစ် သိမ်းထားသည့် part တွင် ပြောင်းလဲထားသည်။ ဤ property သည် [radian](https://en.wikipedia.org/wiki/Radian) အဖြစ် angle ကို လက်ခံသည်။ library `math` မှ function `radians()` သည် degree ကို radian သို့ ပြောင်းပေးသည်။

Property `Rotation.Angle` သည် part ၏ လက်ရှိ placement axis ကို အသုံးပြုသည် (ဤဥပမာတွင် X-axis ဖြစ်သည်)။ part ကို ဥပမာအားဖြင့် Z-axis အပေါ် လှည့်လိုပါက rotation command ကို ခေါ်မီအဘွေ့ rotation axis ကို အောက်ပါ command ဖြင့် သတ်မှတ်နိုင်သည်။



Parts များကို လှည့်ခြင်း အစား ကူးရွှေ့လှည့်လိုပါက ဥပမာ wheel ၏ Y-direction တွင် placement ကို ပြောင်းမည်ဆိုပါက command သည် ဤနေရာတွင် ဖြစ်မည်။



ဤအမှုအရာတွင် `angle` အစား `PositionShift` ဆိုသည့် variable ကို သတ်မှတ်ပြီး loop အစဉ်တိုင်း၌ ပြောင်းလဲသုံးနိုင်သည်။

Part ၏ placement ကို သတ်မှတ်ရန် အမျိုးမျိုးသော နည်းလမ်းများ ရှိသည်။ အချို့ကို [ documented here](Placement.md) တွင် ဖတ်ရှုနိုင်သည်။ ထိုသို့သော် အားလုံးသော placement commands များ၏ စာရင်းကို ယခုအချိန်တွင် မရှိသေးပါ။

A2plus-specific command တစ်ခုရှိသည်။ ၎င်းသည် သင် ယခင်တွင် `document` အဖြစ် ရယူထားသော assembly ၏ constraints များကို ဖြေရှင်းပေးသည်။ `useTransaction` အဖြစ်း ရွေးချယ်ခြင်းသည် FreeCAD ၏ undo/redo stack ထဲသို့ သင့်ပြောင်းလဲမှုအား တစ်ချက်ချင်း သိမ်းဆည်းမည် ဖြစ်ရန် သတ်မှတ်ပေးသည်။ အကြီးမားသော animations များအတွက် ယင်းကို `False` သတ်မှတ်နိုင်သည်။



---
⏵ [documentation index](../README.md) > [Addons](Category_Addons.md) > [External Workbenches](Category_External%20Workbenches.md) > A2plus Workbench