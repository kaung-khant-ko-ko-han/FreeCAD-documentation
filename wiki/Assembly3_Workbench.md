# <img alt="Assembly3 workbench icon" src=images/Assembly3_workbench_icon.svg  style="width:64px;"> Assembly3 Workbench

 
## Introduction

<img alt="" src=images/Assembly3_workbench_icon.svg  style="width:24px;"> [Assembly3](Assembly3_Workbench.md) သည် တစ်ဖိုင်အတွင်း သို့မဟုတ် မျိုးစုံသော မှတ်တမ်းများအတွင်း ပါဝင်သော အစိတ်အပိုင်းများကို တပ်ဆင်စုစည်းရန် အသုံးပြုသော [external workbench](External_workbenches.md) တစ်ခု ဖြစ်သည်။ ဤလုပ်ငန်းခွင်(Workbench) ကို ဖန်တီးရာတွင် FreeCAD 0.19 ဗားရှင်းအတွက် ပြုလုပ်ထားသည့် အဓိကလုပ်ဆောင်ချက် ပြောင်းလဲမှုများအပေါ် အခြေခံထားပါသည် (ဥပမာ [App Link](App_Link.md))၊ ထို့ကြောင့် Assembly3 Workbench ကို အရင်ဗားရှင်းများနှင့် အသုံးမပြုနိုင်ပါ။

Assembly3 Workbench ၏ အဓိက လက္ခဏာများမှာ အောက်ပါအတိုင်း ဖြစ်ပါသည်။

-   အမြန်/အပြန်လှန် ဖြေရှင်းသူ (dynamic/interactive solver) — ၎င်းသည် မောင်းနှင်ရာတွင် mouse ဖြင့် အစိတ်အပိုင်းများကို ရွေ့အောင်လုပ်ထားချိန်တွင် solver က တရားဝင် ပစ္စည်းများ၏ ကိုက်ညီမှုကို ကန့်သတ်ပေးနိုင်သည်ကို ဆိုလိုသည်။ ဥပမာ အဘို့ဘီးကို အယ်ခွက် (axis) နှင့် ချိတ်ဆက်ပြီး ဘီးကို mouse ဖြင့် အကောင့်ချိန်တွင် လှုံ့ဆော်နိုင်သည်။
-   links — ဤသည်သည် အစုံတစ်ခုကိုတစ်ခုတည်းသာ အသုံးပြုပြီး (ဥပမာ သံချောင်းတစ်ခုကို) assembly အတွင်း များစွာ တည်နေရာများတွင် အသုံးပြုနိုင်စေပြီး geometry ကို မလုပ်မဟုတ် duplication မလုပ်ဘဲ အသုံးပြုခွင့်ပေးသည်။
-   external links — assembly သာပါတဲ့ freecad စာရွက်တစ်ခုကို ဖန်တီးထား၍ အစိတ်အပိုင်းများအားလုံးကို သီးသန့်ဖိုင်များတွင် သိမ်းဆည်းနိုင်သည်။ ဖိုင်များကို library သို့မဟုတ် ဖိုင်စနစ်အတွင်း ဂဏန်းမျိုးရာနေရာတွင်ထားနိုင်သည်။ တစ်သာသာလိုအပ်ချက်မှာ link ဖန်တီးချိန်၌ ဖိုင်ကို load လုပ်ထားရမည်ဆိုတာသာဖြစ်သည်။ link ဖန်တီးပြီးနောက် ထိုဖိုင်ကို ဖြင့်ထားရမည်ဖြစ်ပြီး ဖိုင်နှင့် ဆိုင်သော links များကို ပြုပြင်ရန် ဖိုင်ကိုဖွင့်ထားရန် လိုအပ်သည်။ Assembly3 သည် လိုအပ်သလို ဖိုင်များကို နောက်ခံတွင် ဖွင့်ပေးခြင်းဖြင့် ဤပြဿနာကို ဖြေရှင်းပေးပါသည်။
-   hierarchical assemblies — အမှန်တကယ် မော်ကွန်းတပ်ဆင်မှုများတွင် sub-assemblies များ ပါဝင်နိုင်သလို၊ ၎င်း sub-assemblies များတွင် ထပ်မံ sub-assemblies များ ပါဝင်နိုင်သည်။
-   assembly freeze — CPU သည် တစ်ပြိုင်နက်လက်ခံနိုင်သည့် ကန့်သတ်ချက်များပမာဏကို အကန့်အသတ်ရှိသဖြင့် assembly ကို freeze ပြုလုပ်ခြင်းဖြင့် ကြီးမားသော assemblies များတွင်တောင် ကန့်သတ်ချက်များကို အသုံးပြုနိုင်စေသည်။ ပြီးပြည့်စုံပြီးသော assembly များ သို့မဟုတ် dynamic ဖြစ်နေစေဖို့ မလိုအပ်သော ကန့်သတ်ချက်များ (ဥပမာ welding, bolting, glue လုပ်ထားသောအစိတ်အပိုင်းများ) ကို freeze ပြုလုပ်လိုက်လျှင် ၎င်းများကို update တွက်ချက်ချက်အတွက် ထည့်စရာမလိုဘဲ Assembly3 solver မှ fixed geometry အနေဖြင့် သတ်မှတ်ပေးမည်။

    :   မှတ်ချက် — ဤပြဿနာအတွက် အခြားနည်းလမ်းများလည်း ရှိနိုင်ပြီး ဥပမာ <img alt="" src=images/Assembly4_workbench_icon.svg  style="width:24px;"> [Assembly4 Workbench](Assembly4_Workbench.md) ကွဲပြားသော ဖြေရှင်းချက်တစ်ခုကို ပေးနိုင်ပါသည်။

[top](#top.md)

### Toolbars

2020 ခုနှစ်မှစ၍ Assembly3 လုပ်ငန်းခွင်တွင် အောက်ပါ toolbars များ ပါဝင်သည်။

#### Main Toolbar 



:   <img alt="" src=images/Assembly_New_Assembly.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_New_Group.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_New_Element.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_Import.svg‎‎  style="width:28px;"><img alt="" src=images/AngleDown.svg‎‎  style="width:14px;"><img alt="" src=images/Assembly3_workbench_icon.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_QuickSolve.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_Move.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_AxialMove.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_QuickMove.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_LockMover.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_TogglePartVisibility.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_Trace.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_AutoRecompute.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_SmartRecompute.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_AutoFixElement.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_AutoElementVis.svg‎‎  style="width:28px;"><img alt="" src=images/AngleDown.svg‎‎  style="width:14px;"><img alt="" src=images/Assembly_Add_Workplane.svg‎‎  style="width:28px;"><img alt="" src=images/AngleDown.svg‎‎  style="width:14px;"><img alt="" src=images/Assembly_TreeItemUp.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_TreeItemDown.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintMultiply.svg‎‎  style="width:28px;">




<div class="mw-collapsible mw-collapsed">


:   The **Main Toolbar** တွင် မကြာခဏအသုံးများသော လုပ်ဆောင်ချက်များကို ဖုံးလွှမ်းသော ကိရိယာများ ပါဝင်သည်။ tooltip များတွင် keyboard shortcut များကို ပြပါမည်။


<div class="mw-collapsible-content toccolours">

  - <img alt="" src=images/Assembly_New_Assembly.svg‎‎  style="width:32px;"> [Create assembly](Assembly3_CreateAssembly.md): Add an assembly folder

  - <img alt="" src=images/Assembly_New_Group.svg‎‎  style="width:32px;"> [Group objects](Assembly3_GroupObjects.md): Group objects

  - <img alt="" src=images/Assembly_New_Element.svg‎‎  style="width:32px;"> [Create element](Assembly3_CreateElement.md): Create element.

  - Import from STEP. This has two settings

  -\* <img alt="" src=images/Assembly_Import.svg‎‎  style="width:32px;"> [Import from STEP](Assembly3_ImportFromSTEP.md): Import STEP files

  -\* <img alt="" src=images/Assembly_ImportMulti.svg‎‎  style="width:32px;"> [Import as multi-document](Assembly3_ImportMultiDocument.md): Import assemblies from STEP into separate documents

  - <img alt="" src=images/Assembly3_workbench_icon.svg‎‎  style="width:32px;"> [Resolve constraints](Assembly3_ResolveConstraints.md): Resolve constraints

  - <img alt="" src=images/Assembly_QuickSolve.svg‎‎  style="width:32px;"> [Quick solve](Assembly3_QuickSolve.md): Quick resolve constraints

  - <img alt="" src=images/Assembly_Move.svg‎‎  style="width:32px;"> [Move part](Assembly3_MovePart.md): Move parts in 3D, this is specific to Assembly3

  - <img alt="" src=images/Assembly_AxialMove.svg‎‎  style="width:32px;"> [Axial move](Assembly3_AxialMove.md): Axial move parts in 3D, this is the classical tool available elsewhere in FreeCAD

  - <img alt="" src=images/Assembly_QuickMove.svg‎‎  style="width:32px;"> [Quick move](Assembly3_QuickMove.md): This will attach the part selected in the tree to the mouse cursor. It will change the position of the part when you click.

  -: Often added parts are stacked upon each other in the origin. Use this function to grab a part you can not see.

  - <img alt="" src=images/Assembly_LockMover.svg‎‎  style="width:32px;"> [Lock mover](Assembly3_LockMover.md): Lock mover for fixed part. Toggle Button. When this is un-selected you can move the parts that have a \"Locked\" constraint.

  - <img alt="" src=images/Assembly_TogglePartVisibility.svg‎‎  style="width:32px;"> [Toggle part visibility](Assembly3_TogglePartVisibility.md): This toggles the visiblity of the selected part on/off.

  -: Note that this differs from using space. Using space with selected items from a sub-assembly in the 3D view often does not behave as expected. Use this function in those cases (or shortcut A-Space)

  - <img alt="" src=images/Assembly_Trace.svg‎‎  style="width:32px;"> [Trace part move](Assembly3_TracePartMove.md): Trace part move (TBD)

  - <img alt="" src=images/Assembly_AutoRecompute.svg‎‎  style="width:32px;"> [Auto recompute](Assembly3_AutoRecompute.md): Auto recompute. Usually enabled.

  -: May be un-selected when repairing constraints or fixing parts where the solver gives a *\"do not converge\"* message (e.g. by turning the part 180deg)

  - <img alt="" src=images/Assembly_SmartRecompute.svg‎‎  style="width:32px;"> [Smart recompute](Assembly3_SmartRecompute.md): Smart recompute. Usually enabled.

  - <img alt="" src=images/Assembly_AutoFixElement.svg‎‎  style="width:32px;"> [Auto fix element](Assembly3_AutoFixElement.md): Element Auto Fixing. Experimental feature in 0.19_pre

  - Element Style. This has two settings

  -\* <img alt="" src=images/Assembly_AutoElementVis.svg‎‎  style="width:32px;"> [Auto element visibility](Assembly3_AutoElementVisibility.md): Auto element visibility

  -\* <img alt="" src=images/Assembly_ShowElementCS.svg‎‎  style="width:32px;"> [Show element coordinate system](Assembly3_ShowElementCS.md): Show element coordinate system

  - Workplane and origin. Adds a workplane, placement or origin. A part must be selected. This has five settings

  -\* <img alt="" src=images/Assembly_Add_Workplane.svg‎‎  style="width:32px;"> [Add workplane](Assembly3_AddWorkplane.md): Add workplane

  -\* <img alt="" src=images/Assembly_Add_WorkplaneXZ.svg‎‎  style="width:32px;"> [Add XZ workplane](Assembly3_AddXZWorkplane.md): Add XZ workplane

  -\* <img alt="" src=images/Assembly_Add_WorkplaneZY.svg‎‎  style="width:32px;"> [Add ZY workplane](Assembly3_AddZYWorkplane.md): Add YZ workplane

  -\* <img alt="" src=images/Assembly_Add_Placement.svg‎‎  style="width:32px;"> [Add placement](Assembly3_AddPlacement.md): Add placement

  -\* <img alt="" src=images/Assembly_Add_Origin.svg‎‎  style="width:32px;"> [Add Origin](Assembly3_AddOrigin.md): Add Origin

  - <img alt="" src=images/Assembly_TreeItemUp.svg‎‎  style="width:32px;"> [Move item up](Assembly3_MoveItemUp.md): Move selected tree item up

  - <img alt="" src=images/Assembly_TreeItemDown.svg‎‎  style="width:32px;"> [Move item down](Assembly3_MoveItemDown.md): Move selected tree item down

  -: Allows to sort Parts, Elements or Constraints in the tree. Element roll over (top to bottom and vice versa). Only works for a single selection.

  - <img alt="" src=images/Assembly_ConstraintMultiply.svg‎‎  style="width:32px;"> [Multiply constraint](Assembly3_MultiplyConstraint.md): Multiply Constraint. This can be selected if multiple parts and suitable Elements are present.

  -: It is used e.g. to assign multiple fasteners of the same type into multiple holes with one constraint.


</div>


</div>

#### Main Constraints Toolbar 



:   <img alt="" src=images/Assembly_ConstraintLock.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintAlignment.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintCoincidence.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintAttachment.svg‎‎  style="width:28px;"><img alt="" src=images/AngleDown.svg‎‎  style="width:14px;"><img alt="" src=images/Assembly_ConstraintAxial.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintSameOrientation.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintMultiParallel.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintAngle.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPerpendicular.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointCoincident.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointInPlane.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointOnLine.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointOnCircle.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointsDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointPlaneDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointLineDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintSymmetric.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintMore.svg‎‎  style="width:28px;">




<div class="mw-collapsible mw-collapsed">


:   အချို့ ကိရိယာများမှာ အခြား ကိရိယာများအတွက် မီနူး အဖြစ် လုပ်ဆောင်ကြပါသည်။


<div class="mw-collapsible-content toccolours">

  - <img alt="" src=images/Assembly_ConstraintLock.svg‎‎  style="width:32px;"> [Locked](Assembly3_ConstraintLock.md): Add an \"Locked\" constraint to fix one or more parts.

  -: သင်သည် part ၏ geometry element တစ်ခုကို ရွေးရွတ်ရမည်။

  -: vertex သို့မဟုတ် edge ကို ဖစ်ရှင်းပါက part သည် ထို vertex သို့မဟုတ် edge ကို ဗဟိုထား၍ ဖြတ်လှန်လှည့်ပတ်နိုင်သည်။

  -: face တစ်ခုကို ဖစ်ရှင်းပါက part ကို အပြည့် lock ပြုလုပ်မည်။

  - <img alt="" src=images/Assembly_ConstraintAlignment.svg‎‎  style="width:32px;"> [Plane Alignment](Assembly3_ConstraintAlignment.md): Add a \"Plane alignment\" constraint to align planar faces of two or more parts.

  -: မျက်နှာပြင်များသည် coplanar သို့မဟုတ် parallel ဖြစ်စေပြီး ရွေးချယ်လျှင် အကွာအဝေးပါနိုင်သည်။

  - <img alt="" src=images/Assembly_ConstraintCoincidence.svg‎‎  style="width:32px;"> [Plane Coincidence](Assembly3_ConstraintCoincidence.md): Add a \"Plane coincidence\" constraint to coincide planar faces of two or more parts.

  -: မျက်နှာပြင်များသည် ၎င်းတို့၏စင်တာတွင် အတူတက်နေပြီး ရွေးချယ်လျှင် အကွာအဝေး ရှိနိုင်သည်။

  - Attachment. This has two settings

  -\* <img alt="" src=images/Assembly_ConstraintAttachment.svg‎‎  style="width:32px;"> [Attachment](Assembly3_ConstraintAttachment.md): Add an \"Attachment\" constraint to attach two parts with the selected geometry elements.

  -\*: ဤကန့်သတ်ချက်သည် ပါဝင်သော အစိတ်အပိုင်းများကို အပြန်အလှန်တစ်စုတည်းအဖြစ် အပြည့်အဝ စောင့်တားပေးသည်။

  -\* <img alt="" src=images/Assembly_ConstraintAttachmentOffset.svg‎‎  style="width:32px;"> [AttachmentOffset](Assembly3_ConstraintAttachmentOffset.md): Same as \"Attachment\" constraint, but maintaining the current relative placement of the involved parts by applying an element offset.

  -\*: ဤကန့်သတ်ချက်သည် ပါဝင်သော အစိတ်အပိုင်းများကို အပြန်အလှန် တိကျစွာ ပြန်ထားပေးသည်။

  - <img alt="" src=images/Assembly_ConstraintAxial.svg‎‎  style="width:32px;"> [Axial Alignment](Assembly3_ConstraintAxial.md): Add an \"Axial alignment\" constraint to align edges/faces of two or more parts.

  -: ဤကန့်သတ်ချက်တွင် လက်ခံနိုင်သော geometry များမှာ

  -:: linear edges, which become collinear,

  -:: planar faces, which are aligned using their surface normal axis,

  -:: and cylindrical face, which are aligned using the axial direction.

  -: မတူညီသော geometry element များကို ပြောစပ် အသုံးပြုနိုင်သည်။

  - <img alt="" src=images/Assembly_ConstraintSameOrientation.svg‎‎  style="width:32px;"> [Same orientation](Assembly3_ConstraintSameOrientation.md): Add a \"Same orientation\" constraint to align faces of two or more parts.

  -: planes များကို rotation အရ တူညီအောင် ရှိအောင် ပြုလုပ်သည်။

  - <img alt="" src=images/Assembly_ConstraintMultiParallel.svg‎‎  style="width:32px;"> [Multi parallel](Assembly3_ConstraintMultiParallel.md): Add a \"Multi parallel\" constraint to make planar faces or linear edges of two or more parts parallel.

  - <img alt="" src=images/Assembly_ConstraintAngle.svg‎‎  style="width:32px;"> [Angle](Assembly3_ConstraintAngle.md): Add an \"Angle\" constraint to set the angle of planar faces or linear edges of two parts.

  - <img alt="" src=images/Assembly_ConstraintPerpendicular.svg‎‎  style="width:32px;"> [Perpendicular](Assembly3_ConstraintPerpendicular.md): Add a \"Perpendicular\" constraint to make planar faces or linear edges of two parts perpendicular.

  - <img alt="" src=images/Assembly_ConstraintPointCoincident.svg‎‎  style="width:32px;"> [Points coincident](Assembly3_ConstraintPointsCoincident.md): Add a \"Point coincident\" constraint to coincide two points in 2D or 3D.

  - <img alt="" src=images/Assembly_ConstraintPointInPlane.svg‎‎  style="width:32px;"> [Point on plane](Assembly3_ConstraintPointInPlane.md): Add a \"Point on plane\" to constrain one or more point onto a plane.

  - <img alt="" src=images/Assembly_ConstraintPointOnLine.svg‎‎  style="width:32px;"> [Point on line](Assembly3_ConstraintPointOnLine.md): Add a \"Point on line\" to constrain a point onto a line in 2D or 3D.

  - <img alt="" src=images/Assembly_ConstraintPointOnCircle.svg‎‎  style="width:32px;"> [Point on circle](Assembly3_ConstraintPointOnCircle.md): Add a \"Point on circle\" to constrain one or more points on to a clyndrical surface defined by a cricle.

  -: သင့်အား အရင်ဆုံး point (မည်သည့် geometry element မဆို point သတ်မှတ်နိုင်သည်) ကို ရွေး၍ ထို့နောက် circle (သို့မဟုတ် cylindrical surface) ကို ရွေးရမည်ဖြစ်သည်။

  -: ထို့နောက် သင် ဆက်လိုလျှင် အပို point များကို ရွေးထပ်ထည့်နိုင်သည်။

  - <img alt="" src=images/Assembly_ConstraintPointsDistance.svg‎‎  style="width:32px;"> [Points distance](Assembly3_ConstraintPointsDistance.md): Add a \"Points distance\" to constrain the distance of two or more points.

  - <img alt="" src=images/Assembly_ConstraintPointPlaneDistance.svg‎‎  style="width:32px;"> [Point plane distance](Assembly3_ConstraintPointPlaneDistance.md): Add a \"Point plane distance\" to constrain the distance between one or more points and a plane.

  - <img alt="" src=images/Assembly_ConstraintPointLineDistance.svg‎‎  style="width:32px;"> [Point line distance](Assembly3_ConstraintPointLineDistance.md): Add a \"Point line distance\" to constrain the distance between a point and a linear edge in 2D or 3D.

  - <img alt="" src=images/Assembly_ConstraintSymmetric.svg‎‎  style="width:32px;"> [Symmetric](Assembly3_ConstraintSymmetric.md): Add a \"Symmetric\" constraint to make geometry elements of two parts symmetric about a plane.

  -: supported elements များမှာ linear edge နှင့် planar face တို့သာ ဖြစ်ပါသည်။

  - <img alt="" src=images/Assembly_ConstraintMore.svg‎‎  style="width:32px;"> [More](Assembly3_ConstraintMore.md): Toggle toolbars for more constraints

  -: အမှန်တကယ် constraint တစ်ခု မဟုတ်ပေမယ့် **Additional Constraints Toolbars** ကို ပြ/ဖျောက် မော်ဒျူး လုပ်ရန် toggle switch တစ်ခုဖြစ်သည်။


</div>


</div>

#### Additional Constraints Toolbars 



:   <img alt="" src=images/Assembly_ConstraintPointDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintEqualAngle.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointsSymmetric.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintGeneral.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintGeneral.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintSymmetricLine.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointsHorizontal.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointsVertical.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintLineHorizontal.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintLineVertical.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintArcLineTangent.svg‎‎  style="width:28px;"> (Assembly3 Constraints2)





:   <img alt="" src=images/Assembly_ConstraintSketchPlane.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintLineLength.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintEqualLength.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintLengthRatio.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintLengthDifference.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintLengthEqualPointLineDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintEqualLineArcLength.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintMidPoint.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintDiameter.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintEqualRadius.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintPointsProjectDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintEqualPointLineDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_ConstraintColinear.svg‎‎  style="width:28px;"> (Assembly3 Sketch Constraints)




<div class="mw-collapsible mw-collapsed">


:   သင်သည် Main Constraints toolbar ပေါ်မှ **<img src="images/Assembly_ConstraintMore.svg‎‎" width=16px> [More](Assembly3_ConstraintMore.md)** ခလုတ်ကို နှိပ်ခြင်းဖြင့် ဤ toolbars များကို ဖွင့်နိုင်ပါသည်။


<div class="mw-collapsible-content toccolours">

  - <img alt="" src=images/Assembly_ConstraintPointDistance.svg‎‎  style="width:32px;"> [Point distance](Assembly3_ConstraintPointDistance.md): Add a \"Point distance\" to constrain the distance of two points in 2D or 3D.

  - <img alt="" src=images/Assembly_ConstraintEqualAngle.svg‎‎  style="width:32px;"> [Equal angle](Assembly3_ConstraintEqualAngle.md): Add an \"Equal angle\" to equate the angles between two lines or normals.

  - <img alt="" src=images/Assembly_ConstraintPointsSymmetric.svg‎‎  style="width:32px;"> [Points symmetric](Assembly3_ConstraintPointsSymmetric.md): Add a \"Points symmetric\" constraint to make two points symmetric about a plane.

  - <img alt="" src=images/Assembly_ConstraintGeneral.svg‎‎  style="width:32px;"> () [Symmetric horizontal](Assembly3_ConstraintSymmetricHorizontal.md): Symmetric horizontal

  - <img alt="" src=images/Assembly_ConstraintGeneral.svg‎‎  style="width:32px;"> () [Symmetric vertical](Assembly3_ConstraintSymmetricVertical.md): Symmetric vertical

  - <img alt="" src=images/Assembly_ConstraintSymmetricLine.svg‎‎  style="width:32px;"> [Symmetric line](Assembly3_ConstraintSymmetricLine.md): Add a \"Symmetric line\" constraint to make two points symmetric about a line.

  - <img alt="" src=images/Assembly_ConstraintPointsHorizontal.svg‎‎  style="width:32px;"> [Points horizontal](Assembly3_ConstraintPointsHorizontal.md): Add a \"Points horizontal\" constraint to make two points horizontal with each other when projected onto a plane.

  - <img alt="" src=images/Assembly_ConstraintPointsVertical.svg‎‎  style="width:32px;"> [Points vertical](Assembly3_ConstraintPointsVertical.md): Add a \"Points vertical\" constraint to make two points vertical with each other when projected onto a plane.

  - <img alt="" src=images/Assembly_ConstraintLineHorizontal.svg‎‎  style="width:32px;"> [Line horizontal](Assembly3_ConstraintLineHorizontal.md):Add a \"Line horizontal\" constraint to make a line segment horizontal when projected onto a plane.

  - <img alt="" src=images/Assembly_ConstraintLineVertical.svg‎‎  style="width:32px;"> [Line vertical](Assembly3_ConstraintLineVertical.md): Add a \"Line vertical\" constraint to make a line segment vertical when projected onto a plane.

  - <img alt="" src=images/Assembly_ConstraintArcLineTangent.svg‎‎  style="width:32px;"> [Arc line tangent](Assembly3_ConstraintArcLineTangent.md): Add an \"Arc line tangent\" constraint to make a line tangent to an arc at the start or end point of the arc.

  - <img alt="" src=images/Assembly_ConstraintSketchPlane.svg‎‎  style="width:32px;"> [Sketch plane](Assembly3_ConstraintSketchPlane.md): Add a \"Sketch plane\" to define the work plane of any draft element inside or following this constraint.

  -: Add an empty \"Sketch plane\" to undefine the previous work plane.

  - <img alt="" src=images/Assembly_ConstraintLineLength.svg‎‎  style="width:32px;"> [Line length](Assembly3_ConstraintLineLength.md): Add a \"Line length\" constrain the length of a non-subdivided Draft.Wire.

  - <img alt="" src=images/Assembly_ConstraintEqualLength.svg‎‎  style="width:32px;"> [Equal length](Assembly3_ConstraintEqualLength.md): Add an \"Equal length\" constraint to make two lines of the same length.

  - <img alt="" src=images/Assembly_ConstraintLengthRatio.svg‎‎  style="width:32px;"> [Length ratio](Assembly3_ConstraintLengthRatio.md): Add a \"Length ratio\" to constrain the length ratio of two lines.

  - <img alt="" src=images/Assembly_ConstraintLengthDifference.svg‎‎  style="width:32px;"> [Length difference](Assembly3_ConstraintLengthDifference.md): Add a \"Length difference\" to constrain the length difference of two lines.

  - <img alt="" src=images/Assembly_ConstraintLengthEqualPointLineDistance.svg‎‎  style="width:32px;"> [Length Equal Point Line Distance](Assembly3_ConstraintLengthEqualPointLineDistance.md): Add a \"Length Equal Point Line Distance\" to constrain the distance

  -: between a point and a line to be the same as the length of a another line.

  - <img alt="" src=images/Assembly_ConstraintGeneral.svg‎‎  style="width:32px;"> ( <img alt="" src=images/Assembly_ConstraintEqualLineArcLength.svg‎‎  style="width:32px;"> )[Equal Line Arc Length](Assembly3_ConstraintEqualLineArcLength.md): Add an \"Equal Line Arc Length\" constraint to make a line of the same length as an arc.

  - <img alt="" src=images/Assembly_ConstraintMidPoint.svg‎‎  style="width:32px;"> [Mid point](Assembly3_ConstraintMidPoint.md): Add a \"Mid point\" to constrain a point to the middle point of a line.

  - <img alt="" src=images/Assembly_ConstraintDiameter.svg‎‎  style="width:32px;"> [Diameter](Assembly3_ConstraintDiameter.md): Add a \"Diameter\" to constrain the diameter of a circle/arc.

  - <img alt="" src=images/Assembly_ConstraintEqualRadius.svg‎‎  style="width:32px;"> [Equal radius](Assembly3_ConstraintEqualRadius.md): Add an \"Equal radius\" constraint to make two circles/arcs of the same radius.

  - <img alt="" src=images/Assembly_ConstraintPointsProjectDistance.svg‎‎  style="width:32px;"> [Points project distance](Assembly3_ConstraintPointsProjectDistance.md): Add a \"Points project distance\" to constrain the distance of two points projected on a line.

  - <img alt="" src=images/Assembly_ConstraintEqualPointLineDistance.svg‎‎  style="width:32px;"> [Equal point line distance](Assembly3_ConstraintEqualPointLineDistance.md): Add an \"Equal point line distance\" to constrain the distance

  -: between a point and a line to be the same as the distance between another point and line.

  - <img alt="" src=images/Assembly_ConstraintColinear.svg‎‎  style="width:32px;"> [Colinear](Assembly3_ConstraintColinear.md): Add a \"Colinear\" constraint to make two lines collinear.


</div>


</div>


:   The **Constraints Toolbars** သည် parts များကို တပ်ဆင်ရာတွင် အသုံးပြုမည့် အဓိက အင်တာဖေ့ စာမျက်နှာ ဖြစ်ပါသည်။
:   မူလတွင် မရရှိနိုင်သလို greyed out ဖြစ်သည်၊ သို့သော် part ၏ face, line သို့မဟုတ် point တစ်ခုခုကို အနည်းဆုံး တစ်ခု ရွေးလိုက်လျှင် အတွင်းကိရိယာများ တက်လာပါမည်။
:   ယေဘုယျအားဖြင့် သင်သည် ချိတ်ဆက်လိုသည့် Element များကို ရွေးထားပြီး ထို့နောက် ကန့်သတ်ချက်အမျိုးအစားကို ရွေးရပါမည်။
:   ကန့်သတ်ချက်များ၏ အထူးပြားပုံများသည် ကန့်သတ်ချက်၏ လက္ခဏာနှင့် ကိုက်ညီမှုများကို ဖော်ပြပေးပါသည်။

    :   ၎င်းတို့သည် 2D/3D ဖြစ်မဖြစ် သို့မဟုတ် 2 ထက်မပိုသော Element များကို ထည့်နိုင်မည်ဟု ဖော်ပြပေးသည်။
:   အသေးစိတ် ဖော်ပြချက်များကို GitHub wiki တွင် တွေ့လိမ့်မည်။

#### Navigation Toolbar 

:   <img alt="" src=images/Assembly_GotoRelation.svg‎‎  style="width:28px;"> <img alt="" src=images/LinkSelect.svg‎‎  style="width:28px;"> <img alt="" src=images/LinkSelectFinal.svg‎‎  style="width:28px;">


<div class="mw-collapsible mw-collapsed">


:   ဤလုပ်ဆောင်ချက်များသည် linked external files များပါသော hierarchy ရှိ assembly များနှင့် အလုပ်လုပ်စဉ် အထူးအသုံးဝင်ပါသည်။


<div class="mw-collapsible-content toccolours">

  - <img alt="" src=images/Assembly_GotoRelation.svg‎‎  style="width:32px;"> [Go to relation](Assembly3_GoToRelation.md): Reveals the Relations group (hidden by default) and selects a relation object.

  - <img alt="" src=images/Std_LinkSelectLinked.svg  style="width:32px;"> [Select linked object](Std_LinkSelectLinked.md): Selects the linked object and switches to its document. <small>(v0.19)</small> 

  - <img alt="" src=images/Std_LinkSelectLinkedFinal.svg  style="width:32px;"> [Select linked final](Std_LinkSelectLinkedFinal.md): Selects the deepest linked object and switches to its document. <small>(v0.19)</small> 


</div>


</div>

#### Measurement Toolbar 



:   <img alt="" src=images/Assembly_MeasurePointDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_MeasurePointLineDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_MeasurePointPlaneDistance.svg‎‎  style="width:28px;"> <img alt="" src=images/Assembly_MeasureAngle.svg‎‎  style="width:28px;">




<div class="mw-collapsible mw-collapsed">


:   The **Measurement toolbar** သည် အရာနှစ်ခုအကြား အကွာအဝေး သို့မဟုတ် ထောင့်ကို တိုင်းတာရန် လုပ်ဆောင်ချက်များကို ပေးသည်။


<div class="mw-collapsible-content toccolours">

  - <img alt="" src=images/Assembly_MeasurePointDistance.svg‎‎  style="width:32px;"> [Measure points](Assembly3_MeasurePoints.md): Add a \"Measure points\" to measure the distance of two points in 2D or 3D.

  - <img alt="" src=images/Assembly_MeasurePointLineDistance.svg‎‎  style="width:32px;"> [Measure point to line](Assembly3_MeasurePointLine.md): Add a \"Measure point to line\" to measure the distance between a point and a linear edge in 2D or 3D.

  - <img alt="" src=images/Assembly_MeasurePointPlaneDistance.svg‎‎  style="width:32px;"> [Measure point to plane](Assembly3_MeasurePointPlane.md): Add a \"Measure point to plane\" to measure the distance between a point and a plane.

  - <img alt="" src=images/Assembly_MeasureAngle.svg‎‎  style="width:32px;"> [Measure angle](Assembly3_MeasureAngle.md): Add a \"Measure angle\" to measure the angle of planar faces or linear edges of two parts.

:   radius သို့မဟုတ် diameter တိုင်းတာရန် function မရှိသေးပါ။
:   measurement tools များသည် part ပြောင်းလဲမှုများကို သက်တမ်းခံနိုင်ပြီး ဥပမာ ကောက်ပတ်တလုံး၏ edge များအကြား အကွာအဝေးကို cube ကို ပြန်အရွယ်ပြောင်းလည်း ထိန်းသိမ်းထားနိုင်သည်။
:   constraints များကဲ့သို့ အကန့်သတ်ချက်များသည် တပြိုင်နက်အချိန်တွင် တွက်ချက်နှင့် update လုပ်ပေးသည်။ အတွင်းက အလုပ်လုပ်ပုံသည် [constraints](#Constraints.md) နှင့် အလွန်ဆင်တူသည်။ အကွာအဝေး သို့မဟုတ် ထောင့်ကို [Elements](#Elements.md) များအကြား တိုင်းတာပြီး [constraints](#Constraints.md) ကဲ့သို့ပင် တွက်ချက်သည်။ tree တွင် ပြသခြင်းလည်း ထိုပင်အတိုင်း ဖြစ်သည်။


</div>


</div>

သင်သလိုမျှ tool bars များကို ပြင်ဆင်၍ တစ်ခုချင်းသိုင်း ကိရိယာများကို ထည့်/ဖယ်ရှားနိုင်သည်။ Toolbars တွင် မတွေ့ရသည့် လုပ်ဆောင်ချက်များအတွက် Assembly3 menu ကို စစ်ဆေးရန် မမေ့ပါနှင့်။

[top](#top.md)

### Constraints

ဒီဇိုင်နာသည် အစိတ်အပိုင်း နှစ်ခု၏ ဆက်ဆံရေးကို ဆန္ဒရှိသည့် အတိုင်း ရရှိစေရန် ကန့်သတ်ချက်များ (Constraints) ကို အသုံးပြုသည်။ မှန်ကန်သည့် ကန့်သတ်ချက်ကို ရွေးချယ်နိုင်ခြင်းမှာ အနုပညာပင်ဖြစ်သည်။ အစစ်အမှန်အားဖြင့် တစ် object နှစ်ခုအကြား မည်သည့် DOF ကို ဖယ်ရှားလိုက်လည်း တစ်ကြိမ်တည်းသာ ဖယ်ရှားသင့်သည်ဟု ဆိုနိုင်သော်လည်း လက်တွေ့တွင် CAD ကိရိယာများတွင် ရွေးထားသော ကန့်သတ်ချက်များကြောင့် over-constrained ဖြစ်လာခြင်းကို တွေ့ရသည်၊ ၎င်းကို ချိတ်ဆက်ဆော့ဝဲများက အဆင့်မြှင့် algorithm များဖြင့် ချိန်ညှိကာ ဖြေရှင်းကြသည်။ Assembly3 သည် over-constraint များကို တွေ့ရှိ၍ တိုက်ရိုက် ထပ်ဆောင်ရန် algorithm များကို အသုံးပြုသော်လည်း အခုချိန်တွင် ထို algorithm များသည် အလွန် parfect မဟုတ်သေးပါ။ ထို့ကြောင့် Assembly3 အသုံးပြုရာတွင် လက်တွေ့တွင် ကန့်သတ်ချက်များကို သုံးစွဲသည့် DOF များကို သတိထားခြင်း၊ ဘာတွေ lock လုပ်ထားပြီး ဘာတွေ မထိနိုင်သေးကြောင်းကို သိရှိထားခြင်းဖြင့် ပြဿနာများကို ကာကွယ်နိုင်သည်။ ဗဟုသုတအရ တစ်ခုချင်း part သည် 6 DOF ထက် မပိုသော constraint များဖြင့် ဆက်သွယ်ထားသင့်သည်။

:   မှတ်ချက် — solver သည် မဖြေရှင်းနိုင်သော ပေါင်းစပ်မှုတစ်ခုနှင့် တွေ့ဆုံပါက error ကို ပြမည်။ ပြဿနာ၏ အကြောင်းရင်းကို solver က ရှာဖွေဖော်ထုတ်ရရန် အလွန်ခက်ခဲသည်၊ ထို့ကြောင့် ထို error မှ တဆင့် မည်သည့်နေရာတွင် ပြဿနာရှိကြောင်း ထင်ရှားစွာ မရှင်းလင်းနိုင်သော အခြေအနေများ ဖြစ်တတ်သည်။ ကြီးမားသော assembly များတွင် ၎င်းသည် စူးစမ်းရှာဖွေရေးကို ရှုပ်ထွေးစေသည်။ ယခုအခါ သည်ကို ရှောင်ရှားဖို့ လွယ်ကူသော နည်းလမ်း မရှိသေးပါ။ သို့ဖြစ်လျင် စနစ်၏ အလုပ်လုပ်ပုံကို ကောင်းစွာနားလည်ထားခြင်း (.e. [Elements](#Elements.md) ကို ကြည့်ပါ), ပါဝင်သော component များကို တိတိကျကျ အမည်ပေးခြင်း နှင့် solver သော current assembly ကို ဖြေရှင်းနေသည့်အချိန်တွင်သာ ထပ်၍ ကန့်သတ်ချက်များ ထည့်ရန်သာ အကြံပြုပါသည်။ ပြဿနာကို တွေ့ဖော်ရာတွင် အထူးကို အသုံးဝင်သည်မှာ constraint တစ်ခုချင်း၏ \"ContextMenu/Deactivate\" လုပ်ဆောင်ချက်ဖြစ်ပါသည်။

Assembly3 Constraints များသည် နှစ်ခု [Elements](#Elements.md) ကြားရှိ အနေအထား သို့မဟုတ် အလှည်းထောင့်ကို ကန့်သတ်ပေးသည်။ တချို့ ကန့်သတ်ချက်များတွင် ၂ခုထက်ပိုသော [Elements](#Elements.md) များနှင့်တင်ဆက်ပြီး အလုပ်လုပ်နိုင်သည်။ [Elements](#Elements.md) တစ်ခုသည် part ၏ face, line/edge သို့မဟုတ် point တစ်ခု ဖြစ်နိုင်သည်။ ယေဘုယျအားဖြင့် ကန့်သတ်ချက်များကို သတ်မှတ်လိုပါက သင်ဧ။ [Elements](#Elements.md) များကို ရွေး၍ ထို့နောက် Constraints [toolbar](#Toolbars.md) မှ ကန့်သတ်ချက်အမျိုးအစားကို ရွေးပါ။

-   6 DOF ကို မြင့်မားစွာ ဖစ်ရှင်းပြုပြီး 0 DOF ကျန်ရစ်စေသည်:
    -   **Lock**: lock ကန့်သတ်ချက်သည် face တစ်ခုအတွက် အားလုံး DOF များကို ဖစ်ရှင်းပမ်းသည်။ ဤသည်ကို assembly တစ်ခုစီတွင် base part တစ်ခုအတွက် အသုံးပြုသင့်သည်။ သင့်အား \"MoveLock\" function ကို (toolbar တွင်) ဖွင့်ထားချင်စရာရှိနိုင်သည်၊ ထို့ကြောင့် part ကို မအမှားဖြင့် ရွေ့လျားနိုင်ခြင်း မရှိစေရန် ဖြစ်သည်။ သာမန်အားဖြင့် part ကို ဖစ်ရှင်းရာတွင် မည်သည့် face/line/point ကို အသုံးပြုမည်ဆိုသည်မှာ အဓိက မဟုတ်ပါ။ သို့သော် lock သည် တိုက်ရိုက် assembly အတွက်သာ သက်ရောက်သည်ကို မှတ်သားပါ (ဥပမာ sub-assembly ဖြစ်ပါက parent assembly သည် မည်သည့် locked part ကို ကျွန်ုပ်တို့ စီမံရန် မလိုအပ်သေး)။
    -   **Attachment**: Element နှစ်ခု၏ coordinate systems ကို အချင်းချင်း တူညီအောင် ပြုလုပ်သည်။ တွက်ချက်အရ ဤလုပ်ဆောင်ချက်သည် အကန့်အသတ်ဆုံး မျိုးဖြစ်သဖြင့် ဖြစ်နိုင်သမျှ အသုံးပြုရန် သင့်တော်သည်။ ထို [elements](#Elements.md) များ အချိုးအကာ မတိကျပါက element properties ကို အသုံးပြု၍ offset များနှင့် angle များကို ဖြည့်ဆည်းနိုင်သည်။
-   5 DOF ကို ဖစ်ရှင်းပြီး 1 DOF ကျန်ရစ်စေသည်:
    -   **Plane Coincident**: Tx, Ty, Tz, Rx, Ry ကို ဖစ်ရှင်းသည်။ မကျန်သော Rz သာ ပျောက်နေသည်။ plane ၏ \"center\" ဖြတ်သန်းသည့် normal အပေါ် တလှည့်လှည့်ခြင်း ကိုသာ ကျန်ရှိစေပါသည်။
-   4 DOF ကို ဖစ်ရှင်းပြီး 2 DOF ကျန်ရစ်စေသည်:
    -   **Axial Alignment**: Tx, Ty, Rx, Ry ကို ဖစ်ရှင်းပေးသည်။ Tz, Rz တို့သာ ခွင့်ပြုသည်။ ၎င်းသည် အပေါ်ယံ ပုံသဏ္ဍာန်၏ axis အပေါ်တွင် လှည့်ပတ်ခြင်းနှင့် အဲဒီ axis အတိုင်း တည်နေရာပြောင်းရွှေ့ခြင်းကို ခွင့်ပြုထားသည်။ အကယ်၍ သင်အတွက်ရှိပါက နှစ်ခုသော *PointOnLine* ကန့်သတ်ချက်များ (နှစ်နေရာ point မတူပါက) က ဤသို့ပင် အပြီးသတ်ရလဒ်ပေးသည်။ \''Colinear\'' ကန့်သတ်ချက်လည်း ထိုပုံစံနှင့် ဆင်တူသည်။
    -   **PointOnLine**: ဤကန့်သတ်ချက်သည် reference line ၏ normal များအပေါ်ရှိ translation နှင့် rotation များကို ဖယ်ရှားပေးသည်။ တစ်ခုသာ ကျန်မှာ line axis အပေါ် translation နှင့် rotation ဖြစ်သည်။
-   3 DOF ကို ဖစ်ရှင်းပြီး 3 DOF ကျန်ရစ်စေသည်:
    -   **Same Orientation**: Rx, Ry, Rz ကို ဖစ်ရှင်းသည်။ T များအားလုံး ကျန်ရှိသည်။
    -   **Points Coincident**: Tx, Ty, Tz ကို ဖစ်ရှင်းသည်။ R များအားလုံး ကျန်ရှိသည်။
    -   **PointOnPoint** ကန့်သတ်ချက်သည် translation 3 ခုကို ဖယ်ရှားပေးသည်။
    -   **Plane Alignment**: Tz, Rx, Ry (plane motion) ကို ဖစ်ရှင်းသည်။ ဤကန့်သတ်ချက်သည် reference plane အပေါ် normal အတိုင်း ရွေ့လျားမှုပေါ် နှင့် plane ၏ အ axis နှစ်ခုပတ်လည် လှည့်ခေါက်မှုနှစ်ခုကို ဖယ်ရှားပေးသည်။
-   2 DOF ကို ဖစ်ရှင်းပြီး 4 DOF ကျန်ရစ်စေသည်:
    -   **Multi Parallel**: Rx, Ry ကို ဖစ်ရှင်းသည်။ T များနှင့် Rz ကျန်သည်။ ဤကန့်သတ်ချက်သည် reference plane ၏ axis နှစ်ခုပတ်လည် လှည့်ခေါက်မှုနှစ်ခုကို ဖယ်ရှားပေးသည်။
-   1 DOF ကို ဖစ်ရှင်းပြီး 5 DOF ကျန်ရစ်စေသည်:
    -   **Points in Plane**: Tz ကို ဖစ်ရှင်းသည်။ ဤကန့်သတ်ချက်သည် reference plane ၏ normal အပေါ်ဖြစ်သော translation ကို ဖယ်ရှားပေးသည်။
    -   **Points Distance**: Element origins အကြား အကွာအဝေးကို ဖစ်ရှင်းပေးသည်။

        :   ဤသည်သည် *Points in Plane* ထက် ပို၍ လွတ်လပ်ခွင့် ထားပေးသည်။

အခြား

-   **Points on Circle**: Tz နှင့် အချို့ Tx, Ty ကို အနည်းငယ် ဖစ်ရှင်းပေးသည်။ အဆိုပါ point translation (သို့မဟုတ် point များစွာ) ကို circle သို့မဟုတ် disk ဒေသပေါ်တွင် ဖျောက်ထားသည်။ သင့်အား circle ကို ဒုတိယအနေဖြင့် ရွေးရမည်။ ဤကန့်သတ်ချက်သည် အားလုံး rotation များအား အခွင့်လွင့်ထားပြီး circle reference plane တွင် translation အနည်းငယ်သာ ခွင့်ပြုသည်။

*: မှတ်ချက် — အောက်ပါ စာရင်းတွင် Tx, Ty, Tz နှင့် Rx, Ry, Rz များကို involved Element များ၏ reference coordinate systems အပေါ် translation နှင့် rotation များကို ဖော်ပြရန် အသုံးပြုထားသည်။ ၎င်းသည် အားလုံး၏ တိကျသည့် သတ်မှတ်ချက် မဟုတ်နိုင်ပေ၊ ဥပမာ line တစ်ခု ပါဝင်ပါက ၎င်းသည် X, Y သို့မဟုတ် အလယ်တန်း အကွာအလတ်တစ်ခုတွင် ရှိမည်ဟု သတ်မှတ်ထားခြင်း မရှိနိုင်ပါ။ ယခုစနစ်ကို သေးငယ်ခြင်းနှင့် နှိုင်းယှဉ်ရလွယ်ကူစေရန် အသုံးပြုထားခြင်းဖြစ်သည်။ ထို့ကြောင့် Z သည် မျက်နှာများပါက ယေဘုယျအားဖြင့် normal direction ကို ကိုယ်စားပြုသည်။ ဖတ်ရှုရ အဆင်ပြေစေရန် သင့်အား ပိုသေချာမြန်ဆန်သော ဖော်ပြချက်ဖြင့် ပြုပြင်လိုပါက လိုလားပါသည်။*

[top](#top.md)

### Elements

Elements သည် Assembly3 workbench တွင် သတ်မှတ်ထားသည့် အထူးသော အဓိပ္ပါယ်ရှိသော term ဖြစ်ပြီး Assembly3 ကို မှန်ကန်စွာ အသုံးပြုရန် ဤ Elements များကို နားလည်ထားခြင်း အလွန် အရေးကြီးသည်။

Element ကို part ၏ 'selectable item' တစ်ခု ဟု တွေးပါ — ဥပမာ face, edge, circle, corner သို့မဟုတ် အခြား point တစ်ခု။ သင်ကန့်သတ်ချက်များ ထည့်သည့်အခါ ရွေးချယ်သည့် အရာများ ဖြစ်ကြသည်။ tree တွင် Assembly folder တစ်ခုတွင် sub-folders သုံးခု ရှိသည်။ 'Parts' နှင့် 'Constraints' သို့ ပြင်ပတွင် 'Elements' ဟူသော folder ရှိပြီး constraint မထည့်သေးသောအခါ၌ ဤ folder သည် ဖွင့်လွတ်တစ်ခုအဖြစ် ရှိနေမည်။ ကန့်သတ်ချက်တစ်ခုထည့်ပါက ဤ constraint သည် နှစ်ခု (သို့မဟုတ် ပို) 的 child nodes များကို ရရှိမည်၊ ၎င်း child nodes များသည် ရွေးထားသည့် 'Elements' ဖြစ်သည်။ ထို့ပြင် ၎င်းတို့သည် 'Elements' folder တွင်လည်း ထည့်သွင်းမည်ဖြစ်ပြီး ၎င်းသည် assembly တွင် အသုံးပြုထားသည့် 모든 Elements များကို စာရင်းတစ်ခုအဖြစ် ဖော်ပြထားသည်။ ကြီးမားသော assembly များတွင် အမည်များကို ပြောင်းရန် (F2 key) သတ်မှတ်ခြင်း လုပ်သင့်သည်။

ဥပမာတစ်ခုကြည့်ကြပါစို့

:   ဖိုင်အသစ်တစ်ခု ဖန်တီး၍ Part workbench မှ cube နှင့် cylinder တို့ကို ထည့်ပါ။ cylinder ကို cube ပေါ်တွင် တင်စီးချင်သည်။ အရင်ဆုံး base part ကို lock ပြုလုပ်ပါ၊ ဤဥပမာတွင် cube ကို base အဖြစ် သတ်မှတ်မည်။ cube ၏ အောက်ဖက် face ကို ရွေးပြီး \"Locked\" ကန့်သတ်ချက် (Constraints [toolbar](#Toolbars.md) မှ ပထမ icon) ကို ရွေးပါ။ cylinder ၏ အပေါ်ဖက် face နှင့် cube ၏ အပေါ်ဖက် face ကို ရွေးပါ။ ထို့နောက် \"Plane Coincident\" constraint ကို ရွေးပါ။ ယခု cylinder သည် cube ထဲသို့ တက်သွားပြီး tree တွင် 'Constraints' အောက်တွင် child nodes နှစ်ခုပါသော leaf အသစ်တစ်ခု ထည့်သွင်းမည်ဖြစ်သည်။ ထို့ပြင် နှစ်ခုသော child nodes များသည် 'Elements' အောက်တွင်လည်း ထည့်သွင်းထားမည်။ သင့် cylinder သည် cube ထဲတွင် တင်ထားနေက င်ား အပေါ်တွင် မရှိလျှင် အောက်ပါပုံစံအတိုင်း ပြုလုပ်ပါ — 'Constraints' အောက်ရှိ child node ကို ရွေး၍ context menu တွင် 'Flip Part' ကို ရွေးပါ။ ယခု cylinder သည် box ပေါ်တွင် တင်ထားမည်။

အဓိက နားလည်ရမည့် အချက်မှာ constraint သည် 'Elements' tree folder ၌ ရှိသည့် Elements များအပေါ် လင့်ခ်များကို အလုပ်လုပ်စေသည်။ ၎င်းကြောင့် parts များကို အစားထိုးသော်လည်း constraint ဖွဲ့စည်းပုံကို ထိန်းသိမ်းထားနိုင်သည်။ ဤအရာကို ဥပမာမရှိဘဲ မလွယ်ကူစွာ မမြင်နိုင်နိုင်ပါ။

ဤဥပမာသို့ ပြန်မရောက်မီ —

:   မှတ်ချက် — cube တွင် \"Locked\" constraint ထည့်ထားမှုရှိသည်ဟု သေချာစေပါက မဟုတ်ရင် ရုပ်ပုံတွင် ဝေယျဉ်မှု ဖြစ်နိုင်သည်။
:   CAD window တွင် cube ၏ အခြား face တစ်ခုကို ရွေးပါ။ ယခု ငါတို့ tree view တွင်သာ အလုပ်လုပ်မည်။ mouse ဖြင့် tree view ထဲတွင် cube ကို ရွေးထားစေပါ။ cube ကို 'Elements' folder ထဲသို့ Drag&Drop လုပ်ပါ။ folder အမည် 'Elements' အပေါ် drop လုပ်ရန် သတိပြုပါ — ဒါဟာ အဓိက ဖြစ်ရမည်။ ထို့နောက် 'Elements' စာရင်းတွင် element အသစ်တစ်ခု ထည့်သွင်းပါသည့် အရာကို မြင်ရမည်။ ထို့နောက် 'Constraints' folder ၌ သင့် cube face ကို ပြထားသည့် child node ကို ရွေး၍ ဖျက်ပါ။ Constraint တွင် element တစ်ခု လိုအပ်မှုရှိ၍ exclamation mark ပြမည်။ သတိပေးချက်က အရေးကြီးတာက constraint အတွင်း element ကို ဖျက်လိုက်လျှင် list ထဲမှ ဖျက်သွားခြင်း မဟုတ်ပါ — အကြောင်းက constraint အတွင်းရှိ element သည် list အတွင်းရှိ element ကို ရည်ညွှန်းသည့် link တစ်ခုသာ ဖြစ်ပါသည်။ ယခု 'Elements' စာရင်းရှိ အသစ်ထည့်ထား element ကို ရယူ၍ 'Plane Coincident' constraint ၌ drag&drop ပြန်ထည့်ပါ။ ယခု cylinder သည် သင့်ရွေးချယ်ထားသော အခြား face သို့ ရွေ့သွားမည်။ cylinder သည် ထပ်မံ inside ဖြစ်လျှင် context menu မှ 'Flip Part' ကို ထပ်ရွေးရနိုင်သည်။

ဤဥပမာမှ constraint ကို ဖျက်ရန်မလိုဘဲ constraint တွင် အသုံးပြုသော Elements များကို ပြောင်းနိုင်သည်ဟု ပြသခဲ့သည်။ အတူတူပုံစံဖြင့် cylinder ကို မည်သည့် part နှင့်မဆို အပြောင်းအလဲ ပြုလုပ်နိုင်သည်။ ဤဥပမာနှင့် ပိုမို ကစားသဖြင့် အောက်ပါ အချက်များကို တွေ့မြင်ရမည် —

-   Element အမည်ကို စာရင်းတွင် ပြောင်းလဲပါက ၎င်း၏ အမည်သည် 모든 Constraints များတွင် ပြောင်းလဲသက်ရောက်မည်။
-   တစ် Element ကို စာရင်းတွင် 여러 constraints တွင် အသုံးပြုနိုင်သည်။
-   Element ၏ Property Window ကို အသုံးပြု၍ **Offsets** များ ထည့်နိုင်သည်။ ဥပမာ၌ cylinder ကို cube မျက်နှာပေါ်တွင် ရွေ့လျားစေမည်။
-   Main toolbar ၌ \"Show Element Coordinate System\" ခလုတ်ကို အသုံးပြု၍ 'ContextMenu/Flip Part' နှင့် 'ContextMenu/Flip Element' ကြိုက်ရာ ပြောင်းလဲမှုများကို ကြည့်ရှုနိုင်သည်။ Property Window တွင် မည်သို့ပြောင်းလဲနေသည့် အရာကို သေချာကြည့်ပါ။
-   Elements စာရင်းထဲ သို့ အရင်တင်ပြီးနောက် constraint ကို ထည့်လိုက်သည့် နည်းလမ်းကို သုံးနိုင်သည် — ဥပမာ Elements အချို့ကို 'Elements List' ထဲသို့ ထည့်၍ (အမည်ပေးခြင်း အထူးအသုံးဝင်သည်၊ ဥပမာ \"Cube Top Face\" သို့မဟုတ် \"Cube Front Face\") ထို့နောက် ကန့်သတ်ချက်ကို တစ်စုံတစ်ရာရွေးခြင်းမပြုဘဲ ထည့်ပါ၊ ၎င်းသည် empty constraint ဖြစ်မည်။ ထို့နောက် 'Elements' list မှ Elements များကို drag လုပ်၍ ထည့်ပါ။ ရလဒ်သည် ပထမဥပမာတွင် သင်လုပ်သည့် အရာနှင့် တူညီပါမည်။ ဤလေ့ကျင့်မှုကို ပြီးလျှင် constraint များသည် Elements များနှင့် မည်သို့ ဆက်ဆံကြောင်း ပိုပြတ်သားစွာနားလည်လာမည်။
-   PropertyWindow/ConstraintType property ထဲတွင် မည်သည့် item ကိုမဆို ရွေးချယ်ခြင်းဖြင့် အကြောင်းအရာရှိ constraint တစ်ခုကို ပြောင်းနိုင်သည်။

[top](#top.md)

## Compatibility

Assembly3 သည် [Assembly2](Assembly2_Workbench.md) မှ အလားအလာရရှိခဲ့သော်လည်း အဲဒီနှင့် ကိုက်ညီမနေပါ။ Assembly2 ဖြင့် ပြုလုပ်ထားသည့် အဟောင်းများရှိပါက FreeCAD 0.16 ကို သက်ဆိုင်ရာ Assembly2 နှင့် အသုံးပြုနေဆဲ ဖြစ်ရန် အကြံပြုပါသည်။

Assembly3 ဖြင့် ဖန်တီးသော မော်ဒယ်များကို သာ Assembly3 workbench ဖြင့်သာ ဖွင့်၍ တည်းဖြတ်ရန်သာ သင့်တော်ပါသည်။

Assembly3 သည် [A2plus](A2plus_Workbench.md) သို့မဟုတ် [Assembly4](Assembly4_Workbench.md) တို့နှင့် ကိုက်ညီမှု မရှိပါ။ တိုင်းထွာထားသော workbench များဖြင့် ဖန်တီးထားသော မော်ဒယ်များကို အဲဒီ respective workbench ဖြင့်သာ ဖွင့်သင့်သည်။

[top](#top.md)

## Installation

[Assembly3 Workbench](Assembly3_Workbench.md) ကို (March 2022 အခြေအနေအရ) [Addon Manager](Std_AddonMgr.md) မှတဆင့် ရနိုင်ပါသည်။ Assembly3 ၏ ဒုတိယပါတီ အားလိုအပ်ချက်များသည် Addon Manager မှ အလိုအလျောက် စီမံပေးမည်ဖြစ်သည်။

#### Alternate installations 

Assembly3 ကို स्थापनाလုပ်ရန် အခြား နည်းလမ်း 2 မျိုး ရှိပါသည်။

-   realthunder မှ ဖန်တီးထားသော FreeCAD fork အထူးဗားရှင်း။ အသေးစိတ် အချက်အလက်များကို [here](https://github.com/realthunder/FreeCAD/releases) တွင် ကြည့်ရှုပါ။ ဤ fork သည် FreeCAD master branch ၏ တိကျသော commit တစ်ခုအပေါ် အခြေခံထားသော်လည်း master branch တွင် မရှိသေးသော အပို features များကိုပါ ဆောင်ထားသည်။ ယင်းသည် တိကျသော development snapshot အပေါ် အခြေခံထားသောကြောင့် master branch သို့ နေ့စဉ် merge လုပ်ခံရသည့် နောက်ဆုံး features များ မပါဝင်နိုင်ပါ။
-   development [AppImage](AppImage.md) — ဤသည်သည် current master branch အပေါ် အခြေခံပြီး Assembly3 အသုံးပြုရန် လိုအပ်သော dependency များ (ဥပမာ SolveSpace solver) ကိုပါ ထည့်သွင်းထားသည်။

AppImage သည် Linux အတွက်သာ အလုပ်လုပ်သောကြောင့် Windows အသုံးပြုသူများအတွက် Assembly3 အခြားတစ်ခုအဖြစ် စမ်းသပ်နိုင်ရန် realthunder ၏ fork ကို စမ်းသပ်ရန် အကြံပြုပါသည်။

[top](#top.md)

## HowTo

### Get Started 

Assembly3 ဖြင့် assembly တစ်ခု ဖန်တီးရန် နည်းလမ်းများ များစွာ ရှိသည်။ အောက်တွင် အလျင်အမြန်နှင့် တိုတောင်းသော နည်းလမ်းတစ်ခုကို ဖော်ပြထားသည်။

:   <img alt="" src=images/Assembly3_Example-GettingStarted.jpg  style="width:600px;">

:   *Getting Started ဥပမာ၏ နောက်ဆုံးရလဒ်။ ပုံတွင် Assembly3 Workbench ရွေးထား၍ နောက်ထပ် toolbars များကို မြင်နိုင်သည်။ tree view ၏ ဘယ်ဘက်ရှိ ထိပ်တန်းရှိ vertical \"TabBar\" သည် standard FreeCAD အတွင်း မပါဝင်သော AddOn Workbench တစ်ခုဖြစ်ပြီး Addon-Manager ဖြင့် ထည့်သွင်းနိုင်သည်။*

-   **<img src="images/Std_New.svg" width=16px> [New](Std_New.md)** ကို နှိပ်၍ ဖရီးကက် (FreeCAD) ဖိုင်အသစ် ဖန်တီးပါ။
-   <img alt="" src=images/Assembly3_workbench_icon.svg  style="width:16px;"> [Assembly3](Assembly3_Workbench.md) လုပ်ငန်းခွင် (Workbench) သို့ ပြောင်းပါ။
-   **<img src="images/Assembly_New_Assembly.svg‎‎" width=16px> [Create assembly](Assembly3_CreateAssembly.md)
** ကို ရွေးပါ။
-   <img alt="" src=images/Workbench_Part.svg  style="width:16px;"> [Part](Part_Workbench.md) workbench သို့ ပြောင်း၍ <img alt="" src=images/Part_Cylinder.svg  style="width:16px;"> [Cylinder](Part_Cylinder.md) နှင့် <img alt="" src=images/Part_Box.svg  style="width:16px;"> [Cube](Part_Box.md) ကို ထည့်ပါ။
-   <img alt="" src=images/Std_Save.svg  style="width:16px;"> [Save](Std_Save.md) ဖြင့် ဖိုင်ကို သင်နှစ်သက်သည့်နာမည်ဖြင့် သိမ်းဆည်းပါ။ <img alt="" src=images/Std_CloseActiveWindow.svg  style="width:16px;"> [Close](Std_CloseActiveWindow.md) ပြီး <img alt="" src=images/Std_Open.svg  style="width:16px;"> [Open\...](Std_Open.md) ဖြင့် ဖိုင်ကို ထပ်မံဖွင့်ပါ။

Tree view သည် အောက်ပါအတိုင်း ဖြစ်သင့်သည် (0.20.pre and Link Branch):

<img alt="" src=images/Assembly3_Example-Tree-01.png  style="width:300px;"> <img alt="" src=images/Assembly3_Example-Tree-02.png  style="width:280px;">

-   ယခု Cylinder နှင့် Cube နှစ်ခုစလုံးကို mouse ဖြင့် *Drag&Drop* လုပ်၍ **Parts** ဖိုလ်ဒါအောက်သို့ တင်ပါ။ ၎င်းများ သည် ထို folder ထဲသို့ ကူးပြောင်းမည်။

    :   ၎င်းသည် အလျင်အမြန်နည်းလမ်းဖြစ်၍ ဤလိုမျိုး ရိုးရှင်းသောကိစ္စများအတွက် သင့်တော်သည်။ link objects ကို အသုံးပြုခြင်းဖြင့် ပိုကောင်းသော နည်းလမ်းတစ်ခုလည်း ရှိသည်။
    :   Cube နှင့် Cylinder ကို ရွေး၍ **<img src="images/Std_LinkMake.svg" width=16px> [Make link](Std_LinkMake.md)** ကို Context menu (-> LinkActions -> MakeLink) သို့မဟုတ် Structure panel မှ ရွေးပါ။
    :   ၎င်းက link objects နှစ်ခု ထည့်လိမ့်မည်။ ထို့နောက် link objects များကို *Drag&Drop* ပြန်လုပ်၍ **Parts** ဖိုလ်ဒါသို့ ထည့်ပါ။
-   Cylinder နှင့် Cube ၏ top surfaces နှစ်ခုကို Ctrl ကို ဆက်ထား၍ (Mac တွင် Cmd) နှိပ်၍ ရွေးပါ။
-   <img alt="" src=images/Assembly3_workbench_icon.svg  style="width:16px;"> [Assembly3](Assembly3_Workbench.md) workbench သို့ ပြန်လည်ရွေးပါ။
-   [Main constraints toolbar](#Main_Constraints_Toolbar.md) မှ **<img src="images/Assembly_ConstraintCoincidence.svg‎‎" width=16px> [Plane Coincidence](Assembly3_ConstraintCoincidence.md)** ကို ရွေးပါ။

ယခု parts များသည် အချိတ်ဆက်သွားပြီး tree သည် အောက်ပါအတည်အကျ ဖြစ်သင့်သည် (0.20.pre and Link Branch):

<img alt="" src=images/Assembly3_Example-Tree-03.png  style="width:300px;"> <img alt="" src=images/Assembly3_Example-Tree-04.png  style="width:280px;">

-   \_Element (နှစ်ခုထဲမှ သို့မဟုတ် တစ်ခု) ကို မျက်နှာချင်းဆိုင် Click နှိပ်၍ Context Menu မှ **Flip Part** ကို ရွေးပါ။

ယခု Cylinder သည် Cube ၏ အပေါ်တွင် တင်ထားသင့်သည်။ အကယ်၍ အဝပြန်လှည့်နေပါက အခြား element ကို Flip Part ပြန်ရွေးပါ။

:   ကြီးမားသော assembly များတွင် လုပ်သင့်သော အရေးကြီးအဆင့်တစ်ခုချို့် — base part ကို Lock လုပ်ခြင်းကို မမေ့ပါနှင့်။
:   ၎င်းသည် constraint များကနေ ကူးနှောင့်မရအောင် part တစ်ခုကို သတ်မှတ်ခြင်းဖြစ်သည်။ ဤဥပမာတွင် **Cube** ကို base အဖြစ် သတ်မှတ်ပါမည်။
    -   Cube ၏ အောက်ဖက် face ကို ရွေးပါ။ အောက်ဖက် face သာ ရွေးထားပါ၊ Cube ทั้งပိတ်မဟုတ်။
    -   [Main constraints toolbar](#Main_Constraints_Toolbar.md) မှ **<img src="images/Assembly_ConstraintLock.svg‎‎" width=16px> [Locked](Assembly3_ConstraintLock.md)** ကို ရွေးပါ။

ပြီးပါပြီ။

ပြီးစီးသည့် assembly tree သည် အောက်ပါအတိုင်း ဖြစ်သင့်သည် (0.20.pre and Link Branch):

<img alt="" src=images/Assembly3_Example-Tree-05.png  style="width:300px;"> <img alt="" src=images/Assembly3_Example-Tree-06.png  style="width:280px;">:

သင့်စိတ်ကြိုက် Locked constraint ကို tree မှ ထိပ်သို့ ရွှေ့နိုင်သည်။ ၎င်းအတွက် [Main toolbar](#Main_Toolbar.md) တွင် **<img src="images/Assembly_TreeItemUp.svg‎‎" width=16px> [Move item up](Assembly3_MoveItemUp.md)** ခလုတ်ကို အသုံးပြုပါ။

**သတိပေးချက်:** external ဖိုင် အသစ်များအားလုံးကို **save**, **close** နှင့် ပြန် **open** လုပ်ထားရန် လိုအပ်သည်၊ အဘယ်ကြောင့်ဆိုသော် Assembly3 သည် အဲဒီဖိုင်ကို ရှာဖွေရန် အကြောင်းပြချက် လိုအပ်ရန်ဖြစ်သည်။

:   ဤအဆင့်ကို မလုပ်ပါက FreeCAD သည် Assembly3 Workbench တွင် file handle မပေးနိုင်ပါ၊ ဤသို့ဖြင့် new part ကို ရှာမတွေ့နိုင်ပါ။
:   အားလုံး parts များသည် တစ်ဖိုင်တွဲတွင် ရှိပါကလည်း ထိုဖိုင်ကို **save**, **close** နှင့် ပြန် **open** လုပ်ရန် မမေ့ပါနှင့်။

[top](#top.md)

### Add an Offset 

Assembly3 သည် [A2plus Workbench](A2plus_Workbench.md) သို့မဟုတ် အခြား CAD ကိရိယာများကဲ့သို့ Constraint တွင် Offset ကို တိုက်ရိုက် ပံ့ပိုးပေးမှု မရှိသော်လည်း၊ ပို၍ ယေဘုယျနှင့် ချောမွေ့သော စနစ်တစ်ခုဖြင့် translation များနှင့် angle များကို ထည့်သွင်းနိုင်သည့် အင်္ဂါရပ်ကို ပေးထားပါသည်။

-   Offset ကို [Elements](#Elements.md) တစ်ခု၏ properties တွင် ထည့်ပါ။

    :   သင်သည် ထိုနှစ်ခုထဲမှ မည်သည့် element ကို အသုံးချမည်ဆိုတာရွေးနိုင်သည်။

ဥပမာ:

-   Assembly တွင် ကုလပ် 2 ခု ထည့်၍ ၎င်းတို့၏ ဘေးဖက် မျက်နှာများကို ရွေးပါ။
-   \"PlaneCoincident\" ကို ရွေးပါ။ ကုလပ်များသည် အချင်းချင်းထဲတွင် တပ်ဆင်သွားမည်။
-   Element တစ်ခုကို ရွေး၍ *ContextMenu/Flip Part* ကို လုပ်ပါ။ ကုလပ်များသည် ဘေးဘက်တလျှောက် တပ်ဆင်မည်။
-   Element ၏ property ထဲမှ Offset/Position/Zz ကို ရွေး၍ 5mm ဟု သတ်မှတ်ပါ။ ကုလပ်များသည် 5mm အကွာလောက် ဆက်ထားမည်။

  - အခြား axis များနှင့် angle/axis field များကို စမ်းသပ်ကြည့်ပါ။ အခြား Element ကို အသုံးပြုပါကလည်း အလားတူရလဒ် လက်ခံရမည်။ ဤနည်းပညာသည် အခြား constraints အားလုံးတွင်လည်း တူညီသည်။

[top](#top.md)

### Solve a Solver Failure 

ဤအခြေအနေသည် မကြာခဏ over-constrained ဖြစ်သောအခါ ဖြစ်တတ်သည်၊ တမင် 6 DOF ထက်ပို၍ lock လုပ်ထားခြင်းကြောင့် ဖြစ်သည်။

ပြဿနာရှိသော constraint များကို ရှာဖွေရန် အလျြင်ဆုံးနည်းလမ်းမှာ tree ထဲတွင် သက်ဆိုင်ရာ constraints များကို click လုပ်၍ *ContextMenu/Disable* ကို ရွေး၍ ပြန်တွက်ချက်ခြင်း ဖြစ်သည်။ solver မပျက်မကွက် ဖြစ်မှီ ထိပ်ဆုံးထည့်သွင်းခဲ့သော constraint များကို ကြည့်ရှု၍ undo ပြုလုပ်ခြင်းက အထောက်အကူ ဖြစ်နိုင်သည်။

မှတ်ချက် — Assembly3 သည် over-constraint များကို အတွင်းသို့ ကြိုးစား၍ ဖြေရှင်းခင်းချိန်တွင် ပြဿနာသည် အချို့အခါ သင်ထပ်မံထည့်သည့် constraint တစ်ခု ဒီလိုဖြစ်စေသည်၊ သို့သော် အမြစ်ပြဿနာသည် အခြားနေရာ၌ ရှိနိုင်သည်။ အားလုံးကို ဖျက်၍ ပြန်စတင်ခြင်းမပြုမီ Elements များကို ထပ်အသုံးပြုနိုင်ကြောင်း မှတ်သားပါ။ သင့်အား အမည်ပေးထားပါက လိုအပ်သော element များကို ရှာကာ constraints များကို 3D view ကို မသုံးဘဲ ပြန်လည်ဆောက်နိုင်သည်။ အထက်တွင် ဖော်ပြထားသည့် [Elements](#Elements.md) အပိုင်းကို ကြည့်ပါ။

[top](#top.md)

### Replace a part or rename a filename 

Part တစ်ခုကိုဖျက်လိုက်သို့မဟုတ် filename ပြောင်းလိုက်ပါက assembly သည် ပျက်ကွက်သွား၍ solver သည် \"Inconsistent constraints\" ဆိုသည့် 메시ျကို ထုတ်ပေးမည်။ solver သည် tree ၌ မမှန်ကန်သော Elements နှင့် Constraints များကို question mark ဖြင့် အမှတ်အသားပေးမည်။

ဤကို ဖြေရှင်းနိုင်သည့် နည်းလမ်းတစ်ခုမှာ မမှန်ကန်သော constraints နှင့် elements များကို ဖျက်၍ new part ကို import ပြန်ထည့်ပြီး အသစ်ထပ်လုပ်ရခြင်း ဖြစ်သည်။ သို့သော် ပိုကောင်းသော နည်းလမ်းမှာ အောက်ပါအတိုင်း ဖြစ်ပါသည်။

-   ဖိုင်အမည် ပြောင်းခြင်း
    1.  ဖိုင်မန်နေဂျာကို အသုံးပြုပြီး ပြောင်းလိုသော ဖိုင်ကို ကော်ပီ ပြုလုပ်ပါ။ ကော်ပီကို အမည်အသစ်ပေးပါ။
    2.  ကော်ပီကို ဖရီးကက် (FreeCAD) တွင် ဖွင့်ပါ။ နောက်ပိုင်းတွင် assembly နှင့် အဟောင်းဖိုင်ကိုလည်း ဖွင့်ထားရမည်။
    3.  tree မှ အဟောင်း object ကို ရွေး၍ property ထဲရှိ \"Linked object\" ကို ပြောင်းရန် နှိပ်ပါ (၎င်းတွင် အဟောင်း filename ပါရှိမည်)။
    4.  ပြဿနာ dialog တစ်ခု ဖွင့်၍ ဖွင့်ထားသော 모든 parts များကို ပြပါမည်။ အဟောင်း part နှင့် object ကို ရှာဖွေ၍ ရွေးထားမည်။ ပြောင်းလိုက်သော part ကို tree မှ ရှာ၍ အစားထိုးလိုသည့် object ကို ရွေးချယ်၍ confirm ပါ။
    5.  tree ထဲမှ အဟောင်း part ကို ဖျက်ပါ။ ဖိုင်ကိုလည်း ဖျက်နိုင်သည်။
    6.  အဟောင်း part ၏ constraints နှင့် elements များသည် မမှန်ကန်သွားမည်။ tree ၌ constraint သို့မဟုတ် Elements list ကို ဖွင့်ပါ။ ထို့နောက် တစ်ဆင့်ချင်း လုပ်ဆောင်ပါ —
        -   new part ပေါ်ရှိ element surface တစ်ခုကို ရွေးပါ။ tree တွင် item တစ်ခု highlight ဖြစ်ပါမည်။
        -   ထို item ကို သင်ယခင်တွင် အသုံးပြုခဲ့သော အဟောင်း element (Elements list ထဲ သို့မဟုတ် သုံးထားသည့် constraints တစ်ခုအောက်တွင်) အပေါ် drag&drop လုပ်ပါ။ ထို element သည် ထပ်မံ မှန်ကန်လာမည်။
        -   ကျန်သော elements များအတွက် ဤလုပ်ငန်းစဉ်ကို ထပ်မံ လုပ်ဆောင်ပါ။ အများအားဖြင့် element တစ်ခုသာ ဖြစ်စေ Assembly3 သည် အပိုင်း၏ ဖြစ်စဉ်များကို အလိုအလျောက် သက်မှတ်နိုင်သလို ကျန် elements များကို အလိုအလျောက် တွေ့ရှိနိုင်သည်။
        -   အမှားယာ element တစ်ခုကို တားပေးထားခဲ့ပါက ထိုအရာကို မမှန်ကန်ရင် ထပ်မံ နေရာတစ်ခုတွင် တင်ပါ။
    7.  လိုလျှင် FreeCAD တွင် object အမည်ကို ပြောင်းနိုင်သည်။

-   Part တစ်ခုကို အခြား part ဖြင့် အစားထိုးခြင်း

    :   *အဲဒါသည် မူလ part နှင့် ဆင်တူမှု များလုံလောက်၍ မူလ constraints များ အကောင်အထည်ဖော်နိုင်သည့် အခါသာ သက်မှတ်ထားပါ။*

    1.  tree ထဲမှ အဟောင်း part ကို ဖျက်ပါ။ ဖိုင်ကိုလည်း ဖျက်နိုင်သည်။
    2.  အဟောင်း part ၏ constraints နှင့် elements များသည် မမှန်ကန်သွားမည်။ tree ၌ constraint သို့မဟုတ် Elements list ကို ဖွင့်ပါ။
        -   new part ပေါ်ရှိ element surface တစ်ခုကို ရွေးပါ။ tree ၌ item တစ်ခု highlight ဖြစ်မည်။
        -   ထို item ကို အဟောင်း element (Elements list ထဲ သို့မဟုတ် constraints တစ်ခုအောက်တွင်) အပေါ် drag&drop လုပ်ပါ။ ထို element သည် သက်သာသင့်ကျန်ရှင်းလာမည်။
        -   ကျန်သော elements များအတွက် ဤလုပ်ငန်းစဉ်ကို ထပ်မံ လုပ်ပါ။
        -   အမှားယာ element တစ်ခုကို ထပ်မံလေးလှမ်း၍ မှန်ကန်သော surface ကို ထပ်မံ သတ်မှတ်ပါ။
    3.  လိုလျှင် FreeCAD တွင် object အမည်ကို ပြောင်းနိုင်သည်။

''Notes
* ဤလုပ်ငန်းစဉ်များသည် အရွယ်အစားကြီးလှပေမယ့် တတ်တတ်များပြုလုပ်လေ့လာလျှင် 2-3 ကြိမ် အပြီးသတ်ပါက ဒုတိယသဘာဝကဲ့သို့ လွယ်ကူသလောက် ဖြစ်လာမည်။

-   ဤနည်းလမ်းများသည် constraints များကို ဖျက်၍ ပြန်လုပ်ရန် ထက် မြန်ဆန်လွယ်ကူနိုင်သလို လုံခြုံမှုပိုရှိသည်။ အကြောင်းက element တစ်ခုသည် parent assembly တစ်ခုတွင် အသုံးပြုခဲ့နိုင်သဖြင့် မူလ element ကို ဖျက်ခြင်းက အဲဒီ link ကို ပျက်စီးစေမည်ဖြစ်ပြီး ပြန်ချိတ်ဆက်ခြင်းသည် အဲဒီ link ကို သိမ်းဆည်းပေးမည်။
-   constraints နှင့် elements များကို အမည်ပေးထားပါက ဤလုပ်ငန်းစဉ်များသည် အလွန်မြန်ဆန် လွယ်ကူစေမည်။ မည်သည့် surface တွင် drag&drop လုပ်ရမည်ကို အမည်များက ပြောပြထားမည်ဖြစ်ပါသည် (ကြည့်ရန် [Tips & Tricks](#Tips_.26_Tricks.md))။

''

[top](#top.md)

### Tips & Tricks 

-   hierarchical assemblies ကို အသုံးပြုခြင်းဖြင့် solver ပျက်ပြားမှုများကို ရှောင်ရှားနိုင်ပြီး မော်ဒယ်ကို ချောမွေ့စေသည်။ subassembly တစ်ခုကို click တစ်ချက်ဖြင့် freeze ပြုလုပ်၍ CPU resource များကို လွယ်ကူစွာ သိမ်းဆည်းနိုင်သည် (tree ၌ context menu ကို အသုံးပြုပါ)။ Assembly ကို load လုပ်ချိန်တွင် Assembly3 သည် frozen subassemblies များအတွက် external files မဖွင့်သဖြင့် tree ကို လျှော့ချပေးနိုင်သည်။
-   Elements နှင့် constraints များကို အမည်ပေးပေးခြင်းကို အလေ့အကျင့် ပြုပါ။ tree တွင် F2 key ဖြင့် အမြန်ပြောင်းနိုင်သည်။ tree sorting tools များကို main toolbar တွင် ရှာနိုင်သည်။ အမည်ပေးပြီးဖြစ်သော assembly သည် အခြားသူများ သို့မဟုတ် မိမိကိုယ်တိုင် အခြေသက်သက် ကြည့်ရှုသော အခါ လွယ်ကူစွာ နားလည်နိုင်မည်။
    :   ဥပမာ constraint အမည်များအဖြစ် table တစ်လုံးအတွက် \"Align_FrontLegs\", \"Align_FrameBottom-LegTops\" အဖြစ် သတ်မှတ်နိုင်ပြီး element အမည်များကို \"Leg1_Top\" သို့မဟုတ် \"TableTop_Front\", \"TableTop_Left\" စသဖြင့် သတ်မှတ်နိုင်သည်။
-   external files များကို assembly မှ ဖွင့်လိုက်ပြီးနောက် ထိုဖိုင်များကို assembly ကို ပိတ်မခြင်းက ဖွင့်ထားသော files များကို လွယ်ကူစွာ ပိတ်ပစ်ရန် မဖြစ်နိုင်ပါ။ assembly သည် ထိုဖိုင်များကို နောက်ခံတွင် ဖွင့်ထားသဖြင့် tab သည် ပျောက်သွားပေမယ့် file သည် tree တွင် မျက်နှာပြင်အဖြစ် ကျန်ရှိနေပါသည်။ subassemblies အလွှာများရှိလျှင် single files များကို ပိတ်ရန် မလွယ်ကူပါ။ ဤအပြုအမှုကာလအတွင်း workaround အနေနှင့် *File/Save All* နှင့် *File/Close All* ကို ကြာကြာ အသုံးပြု၍ tree ကို သန့်စင်ထားပြီး ကျန်သော sub-assembly တွင် အလုပ်လုပ်ရန် ဖိုင်များကိုသာ ပြန်ဖွင့်သင့်သည်။
    :   ''ဥပမာ — သင်တွင် ကြီးမားသော CNC စက်တစ်ခုရှိပြီး main assembly နှင့် module တစ်ခုချင်းစီအတွက် subassembly များရှိပါက main assembly ကို ဖွင့်လိုက်ရုံမဟုတ်ဘဲ ဘောလုံးတံခြေတစ်ခုအထိ နှစ်ရာကျော်သော files များကို ဖွင့်ရန် ဖြစ်နိုင်သည်။ စက်၏ electronics cabinet subassembly အပေါ် အလုပ်လုပ်ရန်မတိုင်မီ file များအားလုံးကို save & close ပြီး ထပ်မံ ချက်ချင်း အလုပ်လုပ်လိုသည့် subassembly ကိုသာ ဖွင့်ပါ။ ၎င်းသည် မလိုအပ်သော files များကို ဖွင့်ခြင်းမှ ကာကွယ်ပေးပါမည်။''
-   external files အသုံးပြုခြင်းဖြင့် parts များကို ပြန်လည်အသုံးပြုရ လွယ်ကူလာပြီး git သို့မဟုတ် subversion ကဲ့သို့သော versioning စနစ်များဖြင့် part versioning လုပ်နိုင်သည်။ FreeCAD ၏ workflow နှင့် Assembly ကို files အားလုံး တစ်ဖိုင်တည်းထဲထားသည့် လုပ်ငန်းစဉ်နှင့် ဆင်တူသော်လည်း အချို့ အခြေအနေများတွင် single files များဖြင့် အပြန်အလှန် မျှဝေရာတွင် ပိုဆင်လဲအဆင်ပြေတတ်သည်။
-   Multiply linked parts — link ကို assembly တွင် ထည့်ပါက ၎င်းတွင် property value တစ်ခု \"Element Count\" (default 0) ရှိမည်။ ဤကို 3 သတ်မှတ်ပါက အစိတ်အပိုင်း 3 instances ရရှိမည်။ ၎င်းတို့သည် subfolder တစ်ခုအတွင်း ထည့်သွင်းပြီး အပြည့်အစုံ သီးခြား part များကဲ့သို့ အသုံးပြုနိုင်သည်။ ဤ feature ကို အသုံးပြု၍ ဖိုင်၏ ဒေတာ ထောက်လှမ်းမှုကို သက်သာစေပါ — part သည် တစ်ကြိမ်သာ သိမ်းဆည်းပြီး instance တစ်ခုချင်းစီတွင် ကွဲပြားချက်များသာ သိမ်းဆည်းပါမည်။
-   တစ်ချက်နှိပ်ခြင်းဖြင့် မျိုးစုံသော parts (ဥပမာ screws များ) ထည့်သွင်းနိုင်သည် — [Assembly3 Wiki](https://github.com/realthunder/FreeCAD_assembly3/wiki/Constraints-and-Solvers) တွင် ကြည့်ရှုပါ။ ၎င်းသည် အံ့ဩဖွယ် feature အဖြစ်သာမက အသုံးဝင်မှုမြင့်ပါ။
-   [TabBar Workbench](https://github.com/triplus/TabBar) ကို အသုံးပြုခြင်းဖြင့် assembly နှင့် အလုပ်လုပ်ရာတွင် အချိန်လျှော့နိုင်သည်။ ဤ tool သည် workbench တစ်ခုချင်းစီအတွက် ခလုတ်တစ်ခုစီပါဝင်သည့် Toolbar ကို ထည့်ပေးသည်။ သင် toolbar ကို စီစဉ်နိုင်ပြီး သင်လိုရာနေရာတွင် ထားနိုင်သည်။ လူအများစုသည် tree view ၏ ဘယ်ဘက်တွင် ထောင့်ကျောသို့ ထားသည်။ Assembly3, Part, PartDesign နှင့် အခြား အလုပ်များကို မကြာခဏ အသုံးပြုလျှင်၎င်းတို့ကို အမြင့်ဆုံး မျဉ်းတင်ရာတွင်ထားလျှင် workbench switching လုပ်ခြင်း အလွန်လွယ်ကူသည်။

[top](#top.md)

## Links

-   [App Link](App_Link.md) object that makes Assembly3 work.
-   [FreeCAD_assembly3](https://github.com/realthunder/FreeCAD_assembly3) repository and documentation.
-   [Assembly3 preview](https://forum.freecadweb.org/viewtopic.php?f=20&t=25712), big discussion thread.
-   [Tutorial for Assembly 3 Workbench](http://help-freecad-jpg87.fr/02_ass_ind.php) by jpg87.
-   Tutorials about [kinematic assembly](Tutorial_KinematicAssembly.md), [kinematic skeleton](Tutorial_KinematicSkeleton.md), and matching [kinematic controller](Tutorial_KinematicController.md).
-   [Current Assembly Status](https://forum.freecadweb.org/viewtopic.php?f=20&t=34583)
-   [External workbenches](External_workbenches.md)



---
⏵ [documentation index](../README.md) > [Addons](Category_Addons.md) > [External Workbenches](Category_External%20Workbenches.md) > Assembly3 Workbench