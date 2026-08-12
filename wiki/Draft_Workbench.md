# <img alt="Draft workbench icon" src=images/Workbench_Draft.svg  style="width:64px;"> Draft လုပ်ငန်းခွင် (Draft Workbench)

## နိဒါန်း

The <img alt="" src=images/Workbench_Draft.svg  style="width:32px;"> **Draft Workbench** သည် FreeCAD တွင် 2D အရာများ (2D objects) ဖန်တီးခြင်းနှင့် ပြင်ဆင်ခြင်းအပေါ် အဓိက အာရုံစိုက်ထားသည်။ သို့သော် ၎င်းမှာ global coordinate system ၏ XY ပြင် (XY plane) သာ အကန့်သတ်ထားသည့် မဟုတ်ပါ။ Draft အရာများသည် 3D နေရာ၌ မည်သည့် ဗဟိုရေးရာနှင့် တည်နေရာမျှ ရနိုင်ပြီး၊ Draft အရာအချို့ကိုလည်း လွှာပေါ်ရှိ (planar) သို့မဟုတ် မလွှာပေါ် (non‑planar) အဖြစ် သတ်မှတ်နိုင်သည်။

Draft အရာများကို Inkscape သို့မဟုတ် AutoCAD တွင် ပြုလုပ်နိုင်သလို ပုံဆွဲရေးဆိုင်ရာအတော်များများရရှိရန် အသုံးပြုနိုင်သည်။ ထိုအပြင် ၎င်းတို့က အခြား Workbench များတွင် 3D အရာများ ဖန်တီးရာတွင် အခြေခံအဖြစ်အသုံးပြုနိုင်သည်။ ဥပမာ၊ [Draft Wire](Draft_Wire.md) တစ်ခုသည် [Arch Wall](Arch_Wall.md) ၏ path ကို သတ်မှတ်နိုင်ပြီး၊ [Draft Polygon](Draft_Polygon.md) တစ်ခုကို [Part Extrude](Part_Extrude.md) နှင့် extrude ပြုလုပ်နိုင်သည်။ ထို့တပြင် [Draft modifier tools](#Modification.md) များအနက် အများစုကို အခြား workbench များဖြင့် ဖန်တီးထားသော 2D နှင့် 3D အရာများပေါ်တွင်လည်း လျှောက်ထားနိုင်သည်။ ဥပမာ [Sketch](Sketcher_Workbench.md) (စကစ် (Sketch)) ကို [move](Draft_Move.md) လုပ်နိုင်ပြီး၊ [Part](Part_Workbench.md) အရာများမှ [Draft OrthoArray](Draft_OrthoArray.md) တစ်ခုကို ဖန်တီးနိုင်သည်။

Draft Workbench သည် [working plane](Draft_SelectPlane.md) တစ်ခု၊ [grid](Draft_Snap_Grid.md) တစ်ခုနှင့် ဂျီယိုမက္ထရီ၏ တိကျသော တည်နေရာကို ထိန်းချုပ်ပေးနိုင်သော [snapping system](Draft_Snap.md) တို့ကို သတ်မှတ်ပေးသည့် ကိရိယာများလည်း ပံ့ပိုးပေးသည်။

သင်၏ အဓိက ရည်ရွယ်ချက်မှာ ရှုပ်ထွေးသော 2D ပုံစံများနှင့် [DXF](DXF.md) ဖိုင်များ ထုတ်လုပ်ခြင်းသာ ဖြစ်၍ 3D မော်ဒယ်တည်ဆောက်ရန် မလိုအပ်ပါက၊ FreeCAD သည် သင့်လိုအပ်ချက်နှင့် သင့်လျော်မှု မရှိနိုင်ပါ။ ၎င်းအစား လက်ရှိ အထူးပြု 2D drafting ဆော့၀ဲလ်များဖြစ်သော [LibreCAD](https://en.wikipedia.org/wiki/LibreCAD) သို့မဟုတ် [QCad](https://en.wikipedia.org/wiki/QCad) ကဲ့သို့သော အစီအစဉ်များကို စဥ်းစားသင့်နိုင်သည်။

 ![](images/Draft_Workbench_Example.png )  
*ပုံတွင် [grid](Draft_Snap_Grid.md) ကို XY ပြင်နှင့် တန်းစီထားသော အနေအထားကို ပြထားသည်။<br>
ပုံ၏ ဘယ်ဘက်တွင် အဖြူရောင်ဖြင့် များသော planar အရာများကို ပြထားသည်။<br>
ညာဘက်တွင် non‑planar [Draft Wire](Draft_Wire.md) တစ်ခုကို [Draft PathArray](Draft_PathArray.md) ၏ Path Object အဖြစ် အသုံးပြုထားသည်။*

## ပုံကြမ်းရေးဆွဲခြင်း (Drafting)

-   <img alt="" src=images/Draft_Line.svg  style="width:32px;"> [Line](Draft_Line.md): တိုက်ရိုက် တန်းကြောင်း (straight line) တစ်ကြောင်း ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Wire.svg  style="width:32px;"> [Polyline](Draft_Wire.md): polyline (wire ဟုလည်းခေါ်သည်) — တန်းကြောင်း အပိုင်းအစများကို ဆက်သွယ်ထားသည့် အစီအစဉ်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Fillet.svg  style="width:32px;"> [Fillet](Draft_Fillet.md): နှစ်သည့် [Draft Lines](Draft_Line.md) ကြားတွင် ထောင့်များကို မျှဝေစေသော မည်သည့် rounded ထောင့် (fillet) သို့မဟုတ် ဆုတ်လက် ချောင် (chamfer) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Arc.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Arc tools:

  - <img alt="" src=images/Draft_Arc.svg  style="width:32px;"> [Arc](Draft_Arc.md): center၊ radius၊ start angle နှင့် aperture angle မှ တစ်ဆင့် စက်ဝိုင်း arc တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Draft_Arc_3Points.svg  style="width:32px;"> [Arc by 3 points](Draft_Arc_3Points.md): ဝက်ဝိုင်း၏ ထောင့်ကို သတ်မှတ်သည့် အချက်နှစ်သုံးမှ ကိရိယာက ဝက်ဝိုင်း arc တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Circle.svg  style="width:32px;"> [Circle](Draft_Circle.md): center နှင့် radius မှတစ်ဆင့် မိတိကတ် စက်ဝိုင်း တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Ellipse.svg  style="width:32px;"> [Ellipse](Draft_Ellipse.md): ellipse တစ်ခုကို ellipse ထည့်သွင်းနိုင်သော ရက်တန်ဂယ် (rectangle) ကို သတ်မှတ်သည့် နှစ်ချက်မှ ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Rectangle.svg  style="width:32px;"> [Rectangle](Draft_Rectangle.md): နှစ်ချက်မှ ရက်တန်ဂယ်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Polygon.svg  style="width:32px;"> [Polygon](Draft_Polygon.md): center နှင့် radius တိုမှ regular polygon တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_BSpline.svg  style="width:32px;"> [B-spline](Draft_BSpline.md): အချက်များစွာမှ B‑spline curve တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_CubicBezCurve.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Bézier tools:

  - <img alt="" src=images/Draft_CubicBezCurve.svg  style="width:32px;"> [Cubic Bézier curve](Draft_CubicBezCurve.md): တတိယ အဆင့် Bézier curve တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Draft_BezCurve.svg  style="width:32px;"> [Bézier curve](Draft_BezCurve.md): အချက်အချို့မှ Bézier curve တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Point.svg  style="width:32px;"> [Point](Draft_Point.md): အစွန်းတံတစ်ခု (simple point) ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Facebinder.svg  style="width:32px;"> [Facebinder](Draft_Facebinder.md): ရွေးချယ်ထားသော မျက်နှာများမှ မျက်နှာပြင် (surface) အရာတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_ShapeString.svg  style="width:32px;"> [Shape from text](Draft_ShapeString.md): စာသား string တစ်ခုကို ကိုယ်စားပြုသော compound shape တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Hatch.svg  style="width:32px;"> [Hatch](Draft_Hatch.md): ရွေးချယ်ထားသော အရာ၏ planar မျက်နှာများပေါ်တွင် hatches များ ဖန်တီးသည်။

## မှတ်တမ်းထည့်ခြင်း (Annotation)

-   <img alt="" src=images/Draft_Text.svg  style="width:32px;"> [Text](Draft_Text.md): ဖော်ပြရန် အချက်တစ်ချက်တွင် မျိုးစုံစာသား (multi-line text) ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Dimension.svg  style="width:32px;"> [Dimension](Draft_Dimension.md): ရိုးရှင်းသော အကြောင်းအရာ (linear) dimension၊ အချင်းချင်း (radial) dimension သို့မဟုတ် စျေးပုံချိန် (angular) dimension တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Label.svg  style="width:32px;"> [Label](Draft_Label.md): 2-segment leader line နှင့် မြွေတံခါးတစ်ခုပါသည့် မျိုးစုံစာသား တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Draft_AnnotationStyleEditor.svg  style="width:32px;"> [Annotation styles\...](Draft_AnnotationStyleEditor.md): annotation ကဲ့သို့ object များ၏ မြင်ကွင်းဆိုင်ရာ ပROPတီ (visual properties) များကို သတ်မှတ်နိုင်သည့် စတိုင်များကို သတ်မှတ်ရန် ခွင့်ပြုသည်။

## ပြုပြင်ပြောင်းလဲခြင်း (Modification)

-   <img alt="" src=images/Draft_Move.svg  style="width:32px;"> [Move](Draft_Move.md): ရွေးချယ်ထားသော အရာများကို တစ်နေရာမှ အခြားနေရာသို့ တင်ပို့ (move) သို့မဟုတ် ကူးယူ (copy) ပြုလုပ်သည်။

-   <img alt="" src=images/Draft_Rotate.svg  style="width:32px;"> [Rotate](Draft_Rotate.md): center point one ဖက်ပတ်လည် သတ်မှတ်ထားသည့် ဂွမ်းသန်းဖြင့် ရွေးချယ်ထားသော အရာများကို လှည့်ပေးသည် (rotate) သို့မဟုတ် ကူးယူ (copy) ပြုလုပ်သည်။

-   <img alt="" src=images/Draft_Scale.svg  style="width:32px;"> [Scale](Draft_Scale.md): base point အပေါ် အခြေခံ၍ ရွေးချယ်ထားသော အရာများကို အရွယ်ချိန်ညှိ (scale) သို့မဟုတ် ကူးယူ (copy) ပြုလုပ်သည်။

-   <img alt="" src=images/Draft_Mirror.svg  style="width:32px;"> [Mirror](Draft_Mirror.md): ရွေးချယ်ထားသော အရာများမှ ရောင်ပြန် မိတ္တူများ (mirrored copies) ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Offset.svg  style="width:32px;"> [Offset](Draft_Offset.md): ရွေးချယ်ထားသော အရာ၏ တစ်ခုချင်း segment ကို သတ်မှတ်ထားသည့် အကွာအဝေးဖြင့် offset လုပ်ပေး သို့မဟုတ် ရွေးချယ်ထားသော အရာ၏ offset မိတ္တူကို ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Trimex.svg  style="width:32px;"> [Trimex](Draft_Trimex.md): ရွေးချယ်ထားသော အရာကို တိုက်ခတ် (trim) သို့မဟုတ် တိုးချဲ့ (extend) ပြုလုပ်သည်။

-   <img alt="" src=images/Draft_Stretch.svg  style="width:32px;"> [Stretch](Draft_Stretch.md): ရွေးချယ်ထားသော အချက်များကို ရွှေ့ခြင်းဖြင့် အရာများကို တောင့်ချုပ်သည် (stretch)။

-   <img alt="" src=images/Draft_Clone.svg  style="width:32px;"> [Clone](Draft_Clone.md): ရွေးချယ်ထားသော အရာများ၏ linked copies (clones) များကို ဖန်တီးသည်။

-   <img alt="" src=images/Draft_OrthoArray.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Array tools:

  - <img alt="" src=images/Draft_OrthoArray.svg  style="width:32px;"> [Array](Draft_OrthoArray.md): ရွေးချယ်ထားသော အရာမှ orthogonal array တစ်ခု ဖန်တီးသည်။ အလိုအလျောက် [Link](App_Link.md) array တစ်ခုကို ဖန်တီးပေးနိုင်ပါသည်။

  - <img alt="" src=images/Draft_PolarArray.svg  style="width:32px;"> [Polar array](Draft_PolarArray.md): copies များကို ဝက်ဝိုင်းပတ်လမ်းတွင် တပ်ဆင်၍ array တစ်ခု ဖန်တီးသည်။ အလိုအလျောက် [Link](App_Link.md) array ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Draft_CircularArray.svg  style="width:32px;"> [Circular array](Draft_CircularArray.md): concentric ဝက်ဝိုင်းများပေါ်တွင် မိတ္တူများကို တင်ပေးကာ array ဖန်တီးသည်။ အလိုအလျောက် [Link](App_Link.md) array ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Draft_PathArray.svg  style="width:32px;"> [Path array](Draft_PathArray.md): path တစ်ခုအောက်တွင် မိတ္တူများကို တပ်ဆင်ကာ array ဖန်တီးသည်။

  - <img alt="" src=images/Draft_PathLinkArray.svg  style="width:32px;"> [Path link array](Draft_PathLinkArray.md): အထက်ပါအတိုင်း ဖြစ်ပေမယ့် regular array မဟုတ်ဘဲ [Link](App_Link.md) array တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Draft_PointArray.svg  style="width:32px;"> [Point array](Draft_PointArray.md): point compound ၏ အချက်များတွင် မိတ္တူများကို တပ်ဆင်ကာ array ဖန်တီးသည်။

  - <img alt="" src=images/Draft_PointLinkArray.svg  style="width:32px;"> [Point link array](Draft_PointLinkArray.md): အထက်ပါအတိုင်းဖြစ်ပေမယ့် regular array မဟုတ်ဘဲ [Link](App_Link.md) array တစ်ခု ဖန်တီးသည်။

  
-   <img alt="" src=images/Draft_Edit.svg  style="width:32px;"> [Edit](Draft_Edit.md): ရွေးချယ်ထားသော အရာများကို Draft Edit မုဒ်ထဲသို့ ထည့်သည်။ ဤမုဒ်၌ အရာများ၏ properties များကို ဂရပ်ဖစ်ပုံဖြင့် ပြင်ဆင်နိုင်သည်။

-   <img alt="" src=images/Draft_SubelementHighlight.svg  style="width:32px;"> [Subelement highlight](Draft_SubelementHighlight.md): ရွေးချယ်ထားသော အရာများ သို့မဟုတ် ၎င်းတို့၏ base objects များကို ယာယီ highlight ပြုလုပ်သည်။

-   <img alt="" src=images/Draft_Join.svg  style="width:32px;"> [Join](Draft_Join.md): [Draft Lines](Draft_Line.md) နှင့် [Draft Wires](Draft_Wire.md) များကို တစ်ခုတည်း wire တစ်ခုအဖြစ် ပူးစည်းသည်။

-   <img alt="" src=images/Draft_Split.svg  style="width:32px;"> [Split](Draft_Split.md): [Draft Line](Draft_Line.md) သို့မဟုတ် [Draft Wire](Draft_Wire.md) တစ်ခုကို သတ်မှတ်ထားသော အချက် သို့မဟုတ် အနား၌ ခွဲစိတ်သည်။

-   <img alt="" src=images/Draft_Upgrade.svg  style="width:32px;"> [Upgrade](Draft_Upgrade.md): ရွေးချယ်ထားသော အရာများကို upgrade လုပ်သည်။

-   <img alt="" src=images/Draft_Downgrade.svg  style="width:32px;"> [Downgrade](Draft_Downgrade.md): ရွေးချယ်ထားသော အရာများကို downgrade လုပ်သည်။

-   <img alt="" src=images/Draft_WireToBSpline.svg  style="width:32px;"> [Wire to B-spline](Draft_WireToBSpline.md): [Draft Wires](Draft_Wire.md) များကို [Draft BSplines](Draft_BSpline.md) သို့မဟုတ် အနောက်ဘက်သို့ ပြောင်းလဲပေးသည်။

-   <img alt="" src=images/Draft_Draft2Sketch.svg  style="width:32px;"> [Draft to sketch](Draft_Draft2Sketch.md): Draft အရာများအား [Sketcher Sketches](Sketcher_NewSketch.md) သို့မဟုတ် အ inverse ပြောင်းလဲပေးသည်။

-   <img alt="" src=images/Draft_Slope.svg  style="width:32px;"> [Set slope](Draft_Slope.md): ရွေးချယ်ထားသော [Draft Lines](Draft_Line.md) သို့မဟုတ် [Draft Wires](Draft_Wire.md) များ၏ ပထမအချက်နောက်ပိုင်းရှိ အချက်များ အားလုံး၏ Z coordinate ကို မြှင့်/လျော့ချ၍ slope အသတ်မှတ်ပေးသည်။

-   <img alt="" src=images/Draft_FlipDimension.svg  style="width:32px;"> [Flip dimension](Draft_FlipDimension.md): ရွေးချယ်ထားသော [Draft Dimensions](Draft_Dimension.md) များ၏ dimension စာသားကို dimension လိုင်းပတ်လည် 180° လှည့်ပေးသည်။

-   <img alt="" src=images/Draft_Shape2DView.svg  style="width:32px;"> [Shape 2D view](Draft_Shape2DView.md): ရွေးချယ်ထားသော အရာများမှ 2D projection များ ဖန်တီးပေးသည်။

## Draft Tray 

[Draft Tray](Draft_Tray.md) သည် working plane ကို ရွေးချယ်ခြင်း၊ style ဆက်တင်များကို သတ်မှတ်ခြင်း၊ construction mode ကို ပြောင်းသတ်မှတ်ခြင်း၊ နှင့် active layer သို့ group ကို သတ်မှတ်ပေးခြင်းတို့ကို ချုပ်ကိုင်ပေးသည်။

 ![](images/Draft_tray_default.png ) 

-   ![](images/Draft_tray_button_plane.png ) [Select plane](Draft_SelectPlane.md): ယခု Draft working plane ကို သတ်မှတ်သည်။ မီနူးတွင်လည်း ရနိုင်သည်: **Draft → Utilities → <img src="images/Draft_SelectPlane.svg" width=16px> Select Plane**။

-   ![](images/Draft_tray_button_style.png ) [Set style](Draft_SetStyle.md): အရာအသစ်များအတွက် ပုံသဏ္ဍာန် (default style) ကို သတ်မှတ်သည်။ မီနူးတွင်လည်း ရနိုင်သည်: **Draft → Utilities → <img src="images/Draft_SetStyle.svg" width=16px> Set style**။

-   ![](images/Draft_tray_button_construction.png ) [Toggle construction mode](Draft_ToggleConstructionMode.md): Draft construction mode ကို ဖွင့်/ပိတ် ပြောင်းလဲသည်။ မီနူးတွင်လည်း ရနိုင်သည်: **Draft → Utilities → <img src="images/Draft_ToggleConstructionMode.svg" width=16px> Toggle construction mode**။

-   ![](images/Draft_tray_button_layer.png ) [AutoGroup](Draft_AutoGroup.md): active [Draft Layer](Draft_Layer.md) ကို ပြောင်းလဲပေးသည်။ ဝယ်စားလျှင် active [Std Group](Std_Group.md) သို့မဟုတ် group ကဲ့သို့သော [BIM](BIM_Workbench.md) အရာကိုလည်း သတ်မှတ်နိုင်သည်။

  
## Draft annotation scale widget 

[Draft annotation scale widget](Draft_annotation_scale_widget.md) ဖြင့် Draft annotation scale ကို သတ်မှတ်နိုင်သည်။

 ![](images/Draft_annotation_scale_widget_button.png ) 

## Draft snap widget 

[Draft snap widget](Draft_snap_widget.md) သည် [Draft snap toolbar](#Draft_snap_toolbar.md) အစားအတွက် option တစ်ခုအဖြစ် အသုံးပြုနိုင်သည်။

 ![](images/Draft_snap_widget_button.png ) 

## Draft snap toolbar 

Draft snap toolbar သည် active snap options များကို ရွေးချယ်ရန် ခွင့်ပြုသည်။ active option များနှင့် ဆက်စပ်သည့် button များမှာ ဖိထားသည့် အနေအထား (depressed) ဖြင့် ပြထားမည် ဖြစ်သည်။ snapping အကြောင်း အပေါ်ပိုမိုသိရှိလိုပါက: [Draft Snap](Draft_Snap.md) ကို ကြည့်ပါ။

-   <img alt="" src=images/Draft_Snap_Lock.svg  style="width:32px;"> [Snap lock](Draft_Snap_Lock.md): snapping ကို သမ္မာတလျှင် ဖွင့်/ပိတ် လုပ်ပေးသည်။

-   <img alt="" src=images/Draft_Snap_Endpoint.svg  style="width:32px;"> [Snap endpoint](Draft_Snap_Endpoint.md): edge များ၏ endpoint များသို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Midpoint.svg  style="width:32px;"> [Snap midpoint](Draft_Snap_Midpoint.md): edge များ၏ midpoint သို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Center.svg  style="width:32px;"> [Snap center](Draft_Snap_Center.md): face များနှင့် circular edge များ၏ center point များသို့ snap လုပ်ပြီး၊ [Draft WorkingPlaneProxies](Draft_WorkingPlaneProxy.md) နှင့် [Arch BuildingParts](Arch_BuildingPart.md) ၏ **Placement** point များကိုလည်း snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Angle.svg  style="width:32px;"> [Snap angle](Draft_Snap_Angle.md): circular edge များပေါ်ရှိ အထူး cardinal points (30° နှင့် 45° ရှေ့ချိန်များ) အသုံးပြု၍ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Intersection.svg  style="width:32px;"> [Snap intersection](Draft_Snap_Intersection.md): နှစ်ခုသော edge များ၏ အလျားဖြတ်ရာ (intersection) သို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Perpendicular.svg  style="width:32px;"> [Snap perpendicular](Draft_Snap_Perpendicular.md): face (<small>(v0.21)</small>) နှင့် edge များပေါ်ရှိ perpendicular point များသို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Extension.svg  style="width:32px;"> [Snap extension](Draft_Snap_Extension.md): တိုက်ရိုက် edge များ၏ endpoint များကျော်ထွက်သည့် စိတ်ကူးအကြောင်းကြားပေါ်သို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Parallel.svg  style="width:32px;"> [Snap parallel](Draft_Snap_Parallel.md): တိုက်ရိုက် edge များနှင့် ပေပေါ်တွင် parallel ဖြစ်သည့် စိတ်ကူးအကြောင်းကြားပေါ်သို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Special.svg  style="width:32px;"> [Snap special](Draft_Snap_Special.md): အရာအလိုက် သတ်မှတ်ထားသော အထူး အချက်များသို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Near.svg  style="width:32px;"> [Snap near](Draft_Snap_Near.md): face နှင့် edge များပေါ်ရှိ အနီးဆုံး အချက်သို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Ortho.svg  style="width:32px;"> [Snap ortho](Draft_Snap_Ortho.md): နောက်ဆုံး အချက်နှင့် 45° ရာပုံများဖြင့် ထပ်မံဖြတ်ဆိုင်သည့် စိတ်ကူးအကြောင်းကြားပေါ်သို့ snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_Grid.svg  style="width:32px;"> [Snap grid](Draft_Snap_Grid.md): grid line များ၏ ထိမ်း့ချက်များ (intersections) တွင် snap လုပ်သည်။

-   <img alt="" src=images/Draft_Snap_WorkingPlane.svg  style="width:32px;"> [Snap working plane](Draft_Snap_WorkingPlane.md): snap points များကို ယခု [working plane](Draft_SelectPlane.md) သို့ project လုပ်ပေးသည်။

-   <img alt="" src=images/Draft_Snap_Dimensions.svg  style="width:32px;"> [Snap dimensions](Draft_Snap_Dimensions.md): ယာယီ X နှင့် Y dimension များကို ပြသသည်။

-   <img alt="" src=images/Draft_ToggleGrid.svg  style="width:32px;"> [Toggle grid](Draft_ToggleGrid.md): grid ၏ မြင်သာမှုကို ပြောင်းလဲပေးသည်။

## Draft utility tools toolbar 

-   <img alt="" src=images/Draft_LayerManager.svg  style="width:32px;"> [Manage layers\...](Draft_LayerManager.md): document ထဲရှိ layer များကို စီမံခန့်ခွဲရန် ခွင့်ပြုသည်။ <small>(v0.21)</small> 

-   <img alt="" src=images/Draft_AddNamedGroup.svg  style="width:32px;"> [Add a new named group](Draft_AddNamedGroup.md): နာမည်ပါသော [Std Group](Std_Group.md) အသစ်ကို ဖန်တီးပြီး ရွေးချယ်ထားသော အရာများကို ထို group သို့ တင်ပေးသည်။

-   <img alt="" src=images/Draft_AddToGroup.svg  style="width:32px;"> [Move to group\...](Draft_AddToGroup.md): အရာများကို [Std Group](Std_Group.md) သို့ရွှေ့သည်။ အရာများကို ungroup လုပ်ပေးနိုင်မှုလည်း ရှိသည်။

-   <img alt="" src=images/Draft_SelectGroup.svg  style="width:32px;"> [Select group](Draft_SelectGroup.md): [Std Groups](Std_Group.md) သို့မဟုတ် group ကဲ့သို့သော [BIM](BIM_Workbench.md) အရာများ၏ အတွင်းပါ အရာများကို ရွေးချယ်ပေးသည်။

-   <img alt="" src=images/Draft_AddConstruction.svg  style="width:32px;"> [Add to construction group](Draft_AddConstruction.md): အရာများကို [Draft construction group](Draft_ToggleConstructionMode.md) သို့ရွှေ့ပေးသည်။

-   <img alt="" src=images/Draft_ToggleDisplayMode.svg  style="width:32px;"> [Toggle normal/wireframe display](Draft_ToggleDisplayMode.md): ရွေးချယ်ထားသော အရာများ၏ **Display Mode** property ကို {{Value|Flat Lines}} နှင့် {{Value|Wireframe}} အကြား ပြောင်းပေးသည်။

-   <img alt="" src=images/Draft_WorkingPlaneProxy.svg  style="width:32px;"> [Create working plane proxy](Draft_WorkingPlaneProxy.md): ယခု [Draft working plane](Draft_SelectPlane.md) ကို သိမ်းဆည်းရန် working plane proxy တစ်ခု ဖန်တီးသည်။

## အပို ကိရိယာများ (Additional tools) 

**Draft → Utilities** မီနူးတွင် ကိရိယာ များအချို့ပါဝင်သည်။ ၎င်းတို့၏ အများစုကို toolbars များ သို့မဟုတ် [Draft Tray](Draft_Tray.md) မှလည်း ရယူနိုင်ပြီး အထက်တွင် ရှင်းပြထားသည်။ အောက်ပါ ကိရိယာများသည် ထိုရွေးချယ်မှုများတွင် မပါဝင်သော ကိရိယာများဖြစ်သည်။

-   <img alt="" src=images/Draft_ApplyStyle.svg  style="width:32px;"> [Apply current style](Draft_ApplyStyle.md): ယခု style ဆက်တင်များကို ရွေးချယ်ထားသော အရာများပေါ်တွင် လျှောက်ပေးသည်။

-   <img alt="" src=images/Draft_Layer.svg  style="width:32px;"> [Layer](Draft_Layer.md): [Draft Layer](Draft_Layer.md) အသစ်ကို ဖန်တီးသည်။

-   <img alt="" src=images/Draft_Heal.svg  style="width:32px;"> [Heal](Draft_Heal.md): အရမ်းဟောင်းပြီ ဖိုင်များထဲမှ အပြဿနာရှိသော Draft အရာများကို ပြုပြင် (heal) ပေးသည်။

-   <img alt="" src=images/Draft_ShowSnapBar.svg  style="width:32px;"> [Show snap toolbar](Draft_ShowSnapBar.md): [Draft snap toolbar](#Draft_snap_toolbar.md) ကို ပြသသည်။

## အပို လက္ခဏာများ (Additional features) 

-   [Working plane](Draft_SelectPlane.md): အသစ်ပြုလုပ်မည့် Draft အရာများကို ဖန်တီးမည့် [3D view](3D_view.md) အပေါ်ရှိ ဧရိယာ။
-   [Snapping](Draft_Snap.md): ရှိပြီးသား အရာများ သို့မဟုတ် grid မှ သတ်မှတ်ထားသည့် တိကျသော ဂျီယိုမက္ထရီ အချက်များကို ရွေးချယ်ရန်။
-   [Constraining](Draft_Constrain.md): နောက်ထပ် အချက်တစ်ချက်ချင်းစီအတွက် cursor ရှိရာကို X၊ Y သို့မဟုတ် Z ညွှန်ဖြင့် ကန့်သတ်နိုင်သည် (ကန့်သတ်ချက် - Constraint)။
-   [Construction mode](Draft_ToggleConstructionMode.md): အသစ်ဖန်တီးသည့် Draft အရာများကို သီးသန့် group တစ်ခုထဲထားပေးသည့်နည်းဖြင့် ပွ visibility/ဖျက်ပစ်ခြင်းကို အလွယ်တကူ စီမံနိုင်စေသည်။
-   [Pattern](Draft_Pattern.md): **Make Face** property ရှိသော Draft အရာများသည် မီးခိုးရောင်ထက် အစား SVG pattern ကို ပြသနိုင်သည်။

## Tree view context menu 

[Tree view](Tree_view.md) context menu တွင် အောက်ပါ options များ ထပ်မံ ရရှိနိုင်သည်။

### Default options 

Draft အရာအများစုအတွက် အောက်ပါ option ရနိုင်သည် -

-   Edit: အရာကို ပြင်ဆင်သည်။ အရာအမျိုးအစားပေါ် မူတည်၍ [Draft Edit](Draft_Edit.md) သို့မဟုတ် သီးခြား edit ဖြေရှင်းချက်တစ်ခု အသုံးပြုသည်။ <small>(v0.21)</small> 

 document active ဖြစ်သည်ဆိုလျှင် context menu တွင် အပို Utilities sub‑menu တစ်ခု ထပ်ထည့်ထားသည် -

-   Utilities: main Draft Utilities မီနူးတွင် ရရှိနိုင်သည့် ကိရိယာများမှ အပိုင်းတစ်စိတ်တစ်ပိုင်း။

### Layer container options 

[Draft LayerContainer](Draft_Layer.md) အတွက် အောက်ပါ options များ ရနိုင်သည် -

-   <img alt="" src=images/Draft_Layer.svg  style="width:32px;"> [Merge layer duplicates](Draft_Layer#Layer_container_options.md): အခြေခံ label တူသော layer များအားလုံးကို ပေါင်းစည်းပေးသည်။

-   <img alt="" src=images/Draft_NewLayer.svg  style="width:32px;"> [Add new layer](Draft_Layer#Layer_container_options.md): ယခု document တွင် layer အသစ်တစ်ခု ထည့်သွင်းသည်။

### Layer options 

[Draft Layer](Draft_Layer.md) အတွက် အောက်ပါ options များ ရနိုင်သည် -

-   <img alt="" src=images/button_right.svg  style="width:32px;"> [Activate this layer](Draft_AutoGroup.md): ရွေးချယ်ထားသော layer ကို active လုပ်သည်။

-   <img alt="" src=images/Draft_SelectGroup.svg  style="width:32px;"> [Select layer contents](Draft_SelectGroup.md): ရွေးချယ်ထားသော layer အတွင်းရှိ အရာများကို ရွေးချယ်ပေးသည်။

### Text options 

[Draft Text](Draft_Text.md) သို့မဟုတ် hyperlinks (local/remote file သို့ URL) များပါဝင်သော [Draft Label](Draft_Label.md) အတွက် အောက်ပါ အပို option ရရှိနိုင်သည် -

-   Open hyperlinks: hyperlink များကို OS မှ သတ်မှတ်ထားသည့် သင့်တော်သော အပလီကေးရှင်းဖြင့် ဖွင့်သည်။ hyperlinks အများအပြား ရှိပါက သတိပေးချက်တစ်ခု ပေါ်လိမ့်မည်။ <small>(v1.0)</small> 

### Wire options 

[Draft Line](Draft_Line.md) သို့မဟုတ် [Draft Wire](Draft_Wire.md) အတွက် အောက်ပါ option ရနိုင်သည် -

-   <img alt="" src=images/Draft_Edit.svg  style="width:32px;"> Flatten: wire ကို ယခု [Draft working plane](Draft_SelectPlane.md) ပေါ်သို့ flatten ပြုလုပ်သည်။ {{VersionMinus|0.19}} တွင် ဤ option သည် သေချာမဟုတ်ပဲ လုပ်ဆောင်နိုင်သော အတိအကျ ပြဿနာ ရှိနိုင်သည်။

### Working plane proxy options 

[Draft WorkingPlaneProxy](Draft_WorkingPlaneProxy.md) အတွက် အောက်ပါ options များ ရနိုင်သည် -

-   <img alt="" src=images/Draft_SelectPlane.svg  style="width:32px;"> [Write camera position](Draft_WorkingPlaneProxy#Context_menu.md): working plane proxy ၏ **View Data** property ကို ယခု [3D view](3D_view.md) camera သတ်မှတ်ချက်များဖြင့် အဆင့်မြှင့်ရေးထားသည်။

-   <img alt="" src=images/Draft_SelectPlane.svg  style="width:32px;"> [Write objects state](Draft_WorkingPlaneProxy#Context_menu.md): working plane proxy ၏ **Visibility Map** property ကို document အတွင်း objects များ၏ ယခု မြင်သာမှု အခြေအနေဖြင့် အပ်ဒိတ်ပြုလုပ်သည်။

## 3D view context menu 

[3D view](3D_view.md) context menu တွင် အောက်ပါ options များ ထပ်မံရရှိနိုင်သည် -

### Default options 

document active ဖြစ်ပါက context menu တွင် အပို Utilities sub‑menu တစ်ခု ပါရှိသည် -

-   Utilities: main Draft Utilities မီနူးရှိ ကိရိယာများမှ အပိုင်းတစ်စိတ်တစ်ပိုင်း။

### Text options 

အထက်ဖေါ်ပြထားသည့် [Text options](#Text_options.md) ကို ကြည့်ပါ။

## ရှေးခေတ်/အသုံးမကျသော ကိရိယာများ (Obsolete tools) 

-   <img alt="" src=images/Draft_Array.svg  style="width:32px;"> [Array](Draft_Array.md): ရွေးချယ်ထားသော အရာမှ orthogonal array တစ်ခု ဖန်တီးသည်။ ဖန်တီးထားသော array ကို **Array Type** property ပြောင်းလဲခြင်းဖြင့် [polar array](Draft_PolarArray.md) သို့မဟုတ် [circular array](Draft_CircularArray.md) ပြောင်းနိုင်သည်။ <small>(v0.21 တွင် မရရှိနိုင်)</small>။

-   <img alt="" src=images/Draft_Drawing.svg  style="width:32px;"> [Drawing](Draft_Drawing.md): ရွေးချယ်ထားသော အရာများ၏ view များကို [drawing](Drawing_Workbench.md) page ထဲသို့ ထည့်သွင်းသည်။ <small>(v0.21 တွင် မရရှိနိုင်)</small>။

-   <img alt="" src=images/Draft_ToggleContinueMode.svg  style="width:32px;"> [Toggle continue mode](Draft_ToggleContinueMode.md): continue mode ကို ဖွင့်/ပိတ် ပြုလုပ်သည်။ <small>(v1.0 တွင် မရရှိနိုင်)</small>။

## Preferences

-   <img alt="" src=images/Preferences-draft.svg  style="width:32px;"> [Preferences](Draft_Preferences.md): Draft Workbench အတွက် ယေဘုယျချိန်ညှိမှုများ။

-   <img alt="" src=images/Preferences-import-export.svg  style="width:32px;"> [Import Export Preferences](Import_Export_Preferences.md): ဖိုင်ဖော်မတ်များသို့ import/export လုပ်ရာတွင် အသုံးပြုနိုင်သည့် preferences များ။

## ဖိုင်ဖော်မတ်များ (File formats) 

Draft Workbench သည် အချို့သော ဖိုင်ဖော်မတ်များအတွက် FreeCAD အတွင်း importers နှင့် exporters များကို ပံ့ပိုးပေးသည်။ ဤ importers/exporters များကို [Std Import](Std_Import.md) နှင့် [Std Export](Std_Export.md) အမိန့်များမှ အသုံးပြုသည်။

-   [Autodesk .DXF](Draft_DXF.md): [Drawing Exchange Format](http://en.wikipedia.org/wiki/AutoCAD_DXF) (.DXF) ဖိုင်များကို import နှင့် export ပြုလုပ်သည်။ [FreeCAD and DXF Import](FreeCAD_and_DXF_Import.md) ကိုလည်း ကြည့်ပါ။
-   [Autodesk .DWG](Draft_DXF.md): အပြင်ဘက် DWG converter မှတဆင့် DWG ဖိုင်များကို import နှင့် export ပြုလုပ်သည်။ [FreeCAD and DWG Import](FreeCAD_and_DWG_Import.md) ကိုလည်း ကြည့်ပါ။
-   [Scalable Vector Graphics .SVG](Draft_SVG.md): [Scalable Vector Graphics](http://en.wikipedia.org/wiki/Scalable_Vector_Graphics) (.SVG) ဖိုင်များကို import နှင့် export ပြုလုပ်သည်။
-   [Open Cad format .OCA](Draft_OCA.md): [OCA/GCAD](http://groups.google.com/group/open_cad_format) (.OCA) ဖိုင်များကို import နှင့် export ပြုလုပ်သည်။
-   [Airfoil Data Format .DAT](Draft_DAT.md): Airfoil profile များကို ဖော်ပြသည့် .DAT ဖိုင်များကို import ပြုလုပ်သည်။

## ယူနစ် စမ်းသပ်မှုများ (Unit tests) 

လောလောဆယ် ကြည့်ရန်: [Test Workbench](Testing.md)။

Workbench ၏ unit tests များကို operating system terminal မှာ အောက်ပါအတိုင်း အမိန့်ကောက်၍ ပြုလုပ်နိုင်သည်။

```python
freecad -t TestDraft
```

## Scripting

ဆက်လက်ကြည့်ရှုရန်: [Autogenerated API documentation](https://freecad.github.io/SourceDoc/) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

Workbench သည် အသစ် document တစ်ခုတွင် အရာများအားလုံး၏ စမ်းသပ်မှုများ (samples) ဖန်တီးပေးနိုင်သည့် module တစ်ခုကို ပါဝင်သည်။

အရာများအားလုံးမှန်ကန်စွာ ဖန်တီးမိသလား စစ်ဆေးရန် အောက်ပါကို အသုံးပြုပါ -

```python
import drafttests.draft_test_objects as dto
doc = dto.create_test_file()
```

ဤ module ၏ ကုဒ်ကို စစ်ဆေးခြင်းဖြင့် programming interface ကို နားလည်ရန် အထောက်အကူ ဖြစ်နိုင်သည်။

## သင်ခန်းစာများ (Tutorials)

-   [Draft tutorial](Draft_tutorial.md)
-   [Draft ShapeString tutorial](Draft_ShapeString_tutorial.md)



---
⏵ [documentation index](../README.md) > [Workbenches](Category_Workbenches.md) > [Draft](Category_Draft.md) > Draft Workbench