## နိဒါန်း (Introduction)

<img alt="" src=images/Workbench_OpenSCAD.svg  style="width:24px;"> [OpenSCAD လုပ်ငန်းခွင် (OpenSCAD Workbench)](OpenSCAD_Workbench.md) သည် အိုးပင်းဆော့စ် ဆော့ဖ်ဝဲလ်တစ်ခုဖြစ်သော [OpenSCAD](http://www.openscad.org/) နှင့် အပြန်အလှန် ချိတ်ဆက်အသုံးပြုနိုင်ရန် ရည်ရွယ်ပါသည်။ ဤပရိုဂရမ်သည် ဖရီးကက် (FreeCAD) ၏ အစိတ်အပိုင်းတစ်ခုအနေဖြင့် ပါဝင်လာခြင်း မရှိသော်လည်း၊ ဤလုပ်ငန်းခွင်ကို အပြည့်အဝ အသုံးပြုနိုင်ရန်အတွက် ၎င်းကို တပ်ဆင်ထားသင့်ပါသည်။ OpenSCAD ကို ဖရီးကက်မှ မျက်နှာပြင်ပေါ်တွင် ဂျီဩမေတြီ (geometry) များ တည်ဆောက်ရန် အသုံးပြုသော [OpenCASCADE](OpenCASCADE.md) ဂျီဩမေတြီ ကာနယ် (geometrical kernel) နှင့် မရောထွေးသင့်ပါ။ ဖရီးကက်ကို အသုံးပြုရန် OpenCASCADE လိုင်ဘရီများကို အမြဲတမ်း လိုအပ်သော်လည်း၊ OpenSCAD executable ဖိုင်မှာမူ ရွေးချယ်နိုင်သော အရာသာ ဖြစ်ပါသည်။

၎င်းတွင် OpenSCAD မှ CSG ဖိုင်များကို ဖွင့်ရန် [CSG](OpenSCAD_CSG.md) တင်သွင်းမှုစနစ် (importer) နှင့် CSG အခြေခံသော tree တစ်ခုအဖြစ် ထုတ်ယူရန် တင်ပို့မှုစနစ် (exporter) တို့ ပါဝင်သည်။ CSG လုပ်ဆောင်ချက်များအပေါ် အခြေခံမထားသော ဂျီဩမေတြီများကို mesh အဖြစ် တင်ပို့သွားမည် ဖြစ်သည်။

ဤလုပ်ငန်းခွင်တွင် CSG feature tree ကို ပြုပြင်ရန်နှင့် မော်ဒယ်များကို ပြုပြင်ရန် လုပ်ဆောင်ချက်များ ပါဝင်သည်။ ၎င်းတွင် OpenSCAD တပ်ဆင်ရန် မလိုသော ယေဘုယျသုံး ကိရိယာများလည်း ပါဝင်ပြီး ၎င်းတို့ကို အခြားလုပ်ငန်းခွင်များနှင့် တွဲဖက်အသုံးပြုနိုင်ပါသည်။ ဥပမာအားဖြင့်၊ [Mesh လုပ်ငန်းခွင် (Mesh Workbench)](Mesh_Workbench.md) သည် [meshes](mesh.md) များဖြင့် လုပ်ဆောင်ချက်များ ဆောင်ရွက်ရာတွင် အလွန်ခိုင်မာသောကြောင့် OpenSCAD လုပ်ဆောင်ချက်များကို အတွင်းပိုင်းတွင် အသုံးပြုထားပါသည်။

 ![](images/OpenSCADexamaple1.png ) 

## မှီခိုမှုများ (Dependencies)

ဖရီးကက် ၀.၁၉ တွင် CSG ဖိုင်များကို တင်သွင်းရန် အသုံးပြုသော Ply (Python-Lex-Yacc) မော်ဂျူးကို ဖရီးကက်မှ ဖန်တီးထားသော လိုင်ဘရီ မဟုတ်သည့်အတွက် ဖရီးကက်ရင်းမြစ်ကုဒ်မှ ဖယ်ရှားခဲ့ပါသည်။ ရလဒ်အနေဖြင့် OpenSCAD လုပ်ငန်းခွင်ကို အသုံးမပြုမီ Ply ကို တပ်ဆင်ရန် လိုအပ်ပါသည်။ ဖရီးကက်၏ တည်ငြိမ်သောဗားရှင်း (stable version) ကို အသုံးပြုပါက ဤမှီခိုမှုကို အလိုအလျောက် တပ်ဆင်ပေးမည် ဖြစ်သော်လည်း၊ အခြားကိစ္စရပ်များ (ဥပမာ - ရင်းမြစ်ကုဒ်မှ [compile လုပ်ခြင်း (Compiling)](Compiling.md)) တွင် ၎င်းကို အွန်လိုင်းမှ ကိုယ်တိုင်တပ်ဆင်ရနိုင်ပါသည်။

openSUSE တွင် အောက်ပါအတိုင်း လုပ်ဆောင်နိုင်သည် -

```python
sudo zypper install python3-ply
```

Debian/Ubuntu အခြေခံစနစ်များတွင် အောက်ပါအတိုင်း လုပ်ဆောင်နိုင်သည် -

```python
sudo apt install python3-ply
```

အခြား ပလက်ဖောင်းအားလုံးတွင် Python package index မှတစ်ဆင့် ယေဘုယျ တပ်ဆင်မှုကို ပြုလုပ်နိုင်သည် -

```python
pip3 install --user ply
```

## OpenSCAD ဘာသာစကားနှင့် ဖိုင်ပုံစံ (OpenSCAD language and file format)

OpenSCAD ဘာသာစကားသည် ကိန်းရှင်များ (variables) နှင့် ပတ်လမ်းများ (loops) ကို အသုံးပြုခွင့်ပေးသည်။ ၎င်းသည် ဂျီဩမေတြီနှင့် ကုဒ်များကို ပြန်လည်အသုံးပြုရန် sub-modules များ သတ်မှတ်ခြင်းကို ခွင့်ပြုသည်။ ဤသို့ လိုက်လျောညီထွေရှိမှု မြင့်မားခြင်းကြောင့် ကုဒ်များကို ဖတ်ယူရာတွင် (parsing) အလွန်ရှုပ်ထွေးစေပါသည်။ လက်ရှိတွင် OpenSCAD လုပ်ငန်းခွင်သည် OpenSCAD ဘာသာစကားကို တိုက်ရိုက် မကိုင်တွယ်နိုင်သေးပါ။ ယင်းအစား၊ OpenSCAD ကို တပ်ဆင်ထားပါက ၎င်းကို အသုံးပြု၍ OpenSCAD ဘာသာစကား၏ အစိတ်အပိုင်းတစ်ခုဖြစ်သော CSG ပုံစံသို့ ပြောင်းလဲနိုင်ပြီး နောက်ထပ် လုပ်ဆောင်မှုများအတွက် OpenSCAD သို့ ပေးပို့နိုင်ပါသည်။ ပြောင်းလဲနေစဉ်အတွင်း ပါရာမက်ထရစ် (parametric) လုပ်ဆောင်ချက်များ အားလုံး ပျောက်ဆုံးသွားမည်ဖြစ်ပြီး၊ ဆိုလိုသည်မှာ ကိန်းရှင်အမည်များ အားလုံးကို ဖယ်ရှားခြင်း၊ ပတ်လမ်းများကို ဖြန့်ထုတ်ခြင်းနှင့် သင်္ချာဆိုင်ရာ ဖော်ပြချက်များကို တွက်ချက်ခြင်းတို့ ပြုလုပ်သွားမည် ဖြစ်သည်။

## ကိရိယာများ (Tools)

-   <img alt="" src=images/OpenSCAD_ColorCodeShape.svg  style="width:32px;"> [အရောင်ဖြင့် ပုံသဏ္ဌာန် ခွဲခြားခြင်း (Color Code Shape)](OpenSCAD_ColorCodeShape.md): ရွေးချယ်ထားသော သို့မဟုတ် ပုံသဏ္ဌာန် အားလုံး၏ ခိုင်မာမှုအပေါ် မူတည်၍ အရောင်ပြောင်းလဲခြင်း။
-   <img alt="" src=images/OpenSCAD_ReplaceObject.svg  style="width:32px;"> [အရာဝတ္ထု အစားထိုးခြင်း (Replace Object)](OpenSCAD_ReplaceObject.md): feature tree အတွင်းရှိ အရာဝတ္ထုတစ်ခုကို အစားထိုးခြင်း။
-   <img alt="" src=images/OpenSCAD_RemoveSubtree.svg  style="width:32px;"> [Subtree ကို ဖယ်ရှားခြင်း (Remove Subtree)](OpenSCAD_RemoveSubtree.md): ရွေးချယ်ထားသော အရာဝတ္ထုများနှင့် အခြားအရာဝတ္ထုများမှ ရည်ညွှန်းမထားသော child အားလုံးကို ဖယ်ရှားခြင်း။
-   <img alt="" src=images/OpenSCAD_RefineShapeFeature.svg  style="width:32px;"> [ပုံသဏ္ဌာန် အင်္ဂါရပ်ကို သန့်စင်ခြင်း (Refine Shape Feature)](OpenSCAD_RefineShapeFeature.md): မလိုအပ်သော မျဉ်းများကို ရှင်းလင်းခြင်း။
-   <img alt="" src=images/OpenSCAD_MirrorMeshFeature.svg  style="width:32px;"> [Mesh အင်္ဂါရပ်ကို မှန်ပုံရိပ်ဖော်ခြင်း (Mirror Mesh Feature)](OpenSCAD_MirrorMeshFeature.md): Mirror Mesh Feature တစ်ခု ဖန်တီးခြင်း။
-   <img alt="" src=images/OpenSCAD_ScaleMeshFeature.svg  style="width:32px;"> [Mesh အင်္ဂါရပ်ကို စကေးချဲ့ခြင်း (Scale Mesh Feature)](OpenSCAD_ScaleMeshFeature.md): Mesh Feature တစ်ခုကို စကေးချဲ့ခြင်း။
-   <img alt="" src=images/OpenSCAD_ResizeMeshFeature.svg  style="width:32px;"> [Mesh အင်္ဂါရပ်ကို အရွယ်အစား ပြောင်းလဲခြင်း (Resize Mesh Feature)](OpenSCAD_ResizeMeshFeature.md): Mesh Feature တစ်ခုကို အရွယ်အစား ပြောင်းလဲခြင်း။
-   <img alt="" src=images/OpenSCAD_IncreaseToleranceFeature.svg  style="width:32px;"> [Tolerance တိုးမြှင့်ခြင်း အင်္ဂါရပ် (Increase Tolerance Feature)](OpenSCAD_IncreaseToleranceFeature.md): ရွေးချယ်ထားသော အရာဝတ္ထုများ၏ အနားသတ်/မျက်နှာပြင်/ဗားတက်စ် တို့၏ tolerance ကို တိုးမြှင့်ခြင်း။
-   <img alt="" src=images/OpenSCAD_Edgestofaces.svg  style="width:32px;"> [အနားသတ်များကို မျက်နှာပြင်များသို့ ပြောင်းလဲခြင်း (Convert Edges To Faces)](OpenSCAD_Edgestofaces.md): အနားသတ်များကို မျက်နှာပြင်များသို့ ပြောင်းလဲခြင်း။ တင်သွင်းလာသော DXF ဂျီဩမေတြီများကို ထုထည်ထုတ်ရန် (extrusion) ပြင်ဆင်ရာတွင် အသုံးဝင်သည်။
-   <img alt="" src=images/OpenSCAD_ExpandPlacements.svg  style="width:32px;"> [နေရာချထားမှုများကို ဖြန့်ထုတ်ခြင်း (Expand Placements)](OpenSCAD_ExpandPlacements.md): FeatureTree အောက်ခြေအထိ နေရာချထားမှု အားလုံးကို ဖြန့်ထုတ်ခြင်း။
-   <img alt="" src=images/OpenSCAD_ExplodeGroup.svg  style="width:32px;"> [အုပ်စုကို ခွဲထုတ်ခြင်း (Explode Group)](OpenSCAD_ExplodeGroup.md): ပေါင်းစပ်ထားသော part primitives များကို ခွဲထုတ်ခြင်း။
-   <img alt="" src=images/OpenSCAD_AddOpenSCADElement.svg  style="width:32px;"> [OpenSCAD အစိတ်အပိုင်း ထည့်သွင်းခြင်း (Add OpenSCAD Element)](OpenSCAD_AddOpenSCADElement.md): task panel တွင် OpenSCAD ကုဒ်များ ရိုက်ထည့်ခြင်းဖြင့် OpenSCAD အစိတ်အပိုင်းတစ်ခု ထည့်သွင်းခြင်း။
-   <img alt="" src=images/OpenSCAD_MeshBoolean.svg  style="width:32px;"> [Mesh Boolean (Mesh Boolean)](OpenSCAD_MeshBoolean.md): ပုံသဏ္ဌာန်များမှ boolean လုပ်ဆောင်ချက်ဖြင့် mesh အရာဝတ္ထုအသစ် ဖန်တီးခြင်း။
-   <img alt="" src=images/OpenSCAD_Hull.svg  style="width:32px;"> [Hull (Hull)](OpenSCAD_Hull.md): ရွေးချယ်ထားသော ပုံသဏ္ဌာန်များပေါ်တွင် hull တစ်ခု အသုံးပြုခြင်း။
-   <img alt="" src=images/OpenSCAD_Minkowski.svg  style="width:32px;"> [Minkowski (Minkowski)](OpenSCAD_Minkowski.md): ရွေးချယ်ထားသော ပုံသဏ္ဌာန်များပေါ်တွင် minkowski sum တစ်ခု အသုံးပြုခြင်း။

## ဦးစားပေး သတ်မှတ်ချက်များ (Preferences)

-   <img alt="" src=images/Std_DlgPreferences.svg  style="width:32px;"> [ဦးစားပေး သတ်မှတ်ချက်များ (Preferences)](OpenSCAD_Preferences.md): OpenSCAD ကိရိယာများအတွက် ရရှိနိုင်သော ဦးစားပေး သတ်မှတ်ချက်များ။

## ကန့်သတ်ချက်များ (Limitations)

OpenSCAD သည် constructive solid geometry (CSG) ကို ဖန်တီးနိုင်သလို၊ mesh ဖိုင်များကို တင်သွင်းခြင်းနှင့် [DXF](DXF.md) ဖိုင်များမှ ၂ဘက်မြင် ဂျီဩမေတြီများကို ထုထည်ထုတ်ခြင်းတို့ကို ပြုလုပ်နိုင်သည်။ ဖရီးကက်သည်လည်း primitives များဖြင့် CSG ကို ဖန်တီးခွင့်ပေးသည်။ ဖရီးကက်၏ ဂျီဩမေတြီ ကာနယ် (OCCT) သည် boundary representation (BREP) ကို အသုံးပြု၍ အလုပ်လုပ်သည်။ ထို့ကြောင့် CSG မှ BREP သို့ ပြောင်းလဲခြင်းသည် သီအိုရီအရ ဖြစ်နိုင်သော်လည်း၊ BREP မှ CSG သို့ ပြောင်းလဲခြင်းမှာ ယေဘုယျအားဖြင့် မဖြစ်နိုင်ပါ။

OpenSCAD သည် အတွင်းပိုင်းတွင် meshes များပေါ်တွင် အလုပ်လုပ်သည်။ meshes များပေါ်တွင် အသုံးဝင်သော အချို့သော လုပ်ဆောင်ချက်များသည် BREP မော်ဒယ်ပေါ်တွင် အဓိပ္ပာယ်မရှိဘဲ အပြည့်အဝ ထောက်ပံ့မပေးနိုင်ပါ။ ၎င်းတို့ထဲတွင် convex hull, minkowski sum, glide နှင့် subdiv တို့ ပါဝင်သည်။ လက်ရှိတွင် ကျွန်ုပ်တို့သည် hull နှင့် minkwoski လုပ်ဆောင်ချက်များကို ဆောင်ရွက်ရန်နှင့် ရလဒ်ကို တင်သွင်းရန် OpenSCAD binary ကို run ပါသည်။ ဆိုလိုသည်မှာ သက်ဆိုင်ရာ ဂျီဩမေတြီကို triangulated mesh အဖြစ် ပြောင်းလဲသွားမည် ဖြစ်သည်။ OpenSCAD တွင် meshes များကို အသုံးပြုရာတွင် ပြဿနာမရှိသော non-uniform scaling ကို မကြာခဏ အသုံးပြုလေ့ရှိသည်။ ကျွန်ုပ်တို့၏ ဂျီဩမေတြီ ကာနယ်တွင်မူ ထိုသို့သော ပုံပျက်မှုများကို မလုပ်ဆောင်မီ ဂျီဩမေတြီ primitives များ (မျဉ်းများ၊ စက်ဝိုင်းပုံစံများ စသည်) ကို BSpline သို့ ပြောင်းလဲလိုက်သည်။ ထို BSplines များသည် နောက်ပိုင်းတွင် boolean လုပ်ဆောင်ချက်များ ဆောင်ရွက်ရာတွင် ပြဿနာဖြစ်စေနိုင်ကြောင်း သိရှိရပါသည်။ အလိုအလျောက် ဖြေရှင်းပေးမည့် နည်းလမ်းမှာ လက်ရှိတွင် မရှိသေးပါ။ ထိုသို့သော ပြဿနာများ ကြုံတွေ့ရပါက ဖိုရမ်တွင် ပို့စ်တင်နိုင်ပါသည်။ များသောအားဖြင့် ထိုပြဿနာများကို အစိတ်အပိုင်းငယ်များကို ပြန်လည်ပုံဖော်ခြင်းဖြင့် ဖြေရှင်းနိုင်ပါသည်။ ဆလင်ဒါတစ်ခု၏ ပုံပျက်ခြင်းကို ဘဲဥပုံစံ (ellipse) တစ်ခု၏ ထုထည်ထုတ်ခြင်း (extrusion) ဖြင့် အစားထိုးနိုင်ပါသည်။

## စာသားများ တင်သွင်းခြင်း (Importing text)

စာသားများပါဝင်သော OpenSCAD ကုဒ်များကို တင်သွင်းရာတွင် အသုံးပြုထားသော ဖောင့် (fonts) များသည် သင့်စနစ်တွင် မှန်ကန်စွာ တပ်ဆင်ထားရန် လိုအပ်ပါသည်။ ၎င်းကို စစ်ဆေးရန် OpenSCAD ကို သီးသန့်ဖွင့်ပြီး **Help → Font List** တွင် ကြည့်ရှုနိုင်ပါသည်။ ထိုစာရင်းတွင် မှန်ကန်သော ဖောင့်အမည်များကိုလည်း ဖော်ပြပေးမည် ဖြစ်သည်။ ဖောင့်တစ်ခုကို တပ်ဆင်ပြီးနောက် စာရင်းတွင် ပေါ်မလာပါက၊ ဖောင့်ဖိုင်ကို သက်ဆိုင်ရာ စနစ်လမ်းကြောင်း (system directory) သို့ ကိုယ်တိုင် ကူးယူရနိုင်ပါသည်။

စာသားများ တင်သွင်းခြင်းသည် အတော်အတန် နှေးကွေးပါသည်။ ဖရီးကက်သည် နောက်ကွယ်တွင် OpenSCAD မှ ဖန်တီးထားသော DXF ဖိုင်ကို အသုံးပြုပါသည်။ contours များလေလေ တင်သွင်းမှု ပိုနှေးလေလေ ဖြစ်သည်။

ပထမဦးစွာ ရိုးရှင်းသော စမ်းသပ်ချက်တစ်ခုကို တင်သွင်းခြင်းသည် ကောင်းမွန်သော အကြံဉာဏ် ဖြစ်ပါသည် ({{Incode|NameOfFont}} ကို မှန်ကန်သော ဖောင့်အမည်ဖြင့် အစားထိုးပါ) -

    TESTFONT="NameOfFont";
    linear_extrude(0.001) {
      text("A", size=5, font=TESTFONT, script="Latn");
    };

{{Incode|<nowiki>script="Latn"</nowiki>}} ပါရာမီတာကို ဤနေရာတွင် ချန်လှပ်ထားနိုင်သော်လည်း၊ စာသားအတွင်း၌ စာလုံးများ မပါဝင်ဘဲ ပုဒ်ဖြတ်ပုဒ်ရပ် သို့မဟုတ် ကိန်းဂဏန်းများသာ ပါဝင်ပါက လိုအပ်ပါသည်။

ဖရီးကက်သို့ တင်သွင်းရာတွင် သင်၏ ရင်းမြစ်ဖိုင်များရှိ {{Incode|<nowiki>use <FONT>;</nowiki>}} ဖော်ပြချက်များကို လျစ်လျူရှုထားမည်ဖြစ်ကြောင်း သတိပြုပါ။ OpenSCAD အောက်တွင် {{Incode|use}} ဖော်ပြချက်၏ အကျိုးသက်ရောက်မှုမှာ ပေးထားသော ဖောင့်ဖိုင်ကို သိရှိပြီးသား ဖောင့်စာရင်းထဲသို့ ယာယီထည့်သွင်းပေးခြင်း ဖြစ်ပါသည်။

## အရိပ်အမြွက်များ (Hints)

[DXF](DXF.md) ကို တင်သွင်းရာတွင် Draft precision ကို သင့်တော်သော ပမာဏတစ်ခု သတ်မှတ်ပါ၊ အကြောင်းမှာ ၎င်းသည် ဆက်သွယ်ထားသော အနားသတ်များကို ရှာဖွေရာတွင် သက်ရောက်မှု ရှိနိုင်သောကြောင့် ဖြစ်သည်။

CSG ကို တင်သွင်းစဉ် ဖရီးကက် ပျက်ကျပါက (crash)၊ **Menu → Edit → Preferences → Part Design → Model setting** ရှိ \"automatically check model after boolean operation\" ကို ဖွင့်ထားရန် အလေးအနက် အကြံပြုလိုပါသည်။

---
⏵ [မှတ်တမ်း အညွှန်း (documentation index)](../README.md) > [လုပ်ငန်းခွင်များ (Workbenches)](Category_Workbenches.md) > [OpenSCAD](Category_OpenSCAD.md) > OpenSCAD လုပ်ငန်းခွင် (OpenSCAD Workbench)
