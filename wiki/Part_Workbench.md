# <img alt="Part workbench icon" src=images/Workbench_Part.svg  style="width:64px;"> Part Workbench (လုပ်ငန်းခွင်)

## Introduction

The <img alt="" src=images/Workbench_Part.svg  style="width:32px;"> **Part Workbench** (လုပ်ငန်းခွင်) provides a traditional [constructive solid geometry](Constructive_solid_geometry.md) (CSG) workflow. In this workflow each object is an independent solid. The Part Workbench can create them from parametrically defined [sketches](Sketcher_Workbench.md) using tools like [Extrude](Part_Extrude.md), [Revolve](Part_Revolve.md), [Loft](Part_Loft.md), etc. In addition, basic primitive solids like [Cube](Part_Box.md), [Cylinder](Part_Cylinder.md), etc. can be created as well. These objects can be combined, through [Boolean operations](Part_Boolean.md), to create more complex solids.

Part Workbench သည် ရိုးရာ [constructive solid geometry](Constructive_solid_geometry.md) (CSG) လုပ်ငန်းစဉ်တစ်ခုကို ပံ့ပိုးပေးသော Workbench (လုပ်ငန်းခွင်) ဖြစ်သည်။ ဤလုပ်ငန်းစဉ်တွင် အရာဝတ္ထုတစ်ခုချင်းစီကို လွတ်လပ်သော စိုလ်ဓုတိ(သံ)အဖြစ် ကိုင်တွယ်သည်။ Part Workbench သည် parameter ဖြင့် သတ်မှတ်ထားသည့် [sketches](Sketcher_Workbench.md) များမှ [Extrude](Part_Extrude.md), [Revolve](Part_Revolve.md), [Loft](Part_Loft.md) စသည့် ကိရိယာများအား အသုံးပြု၍ အဆိုပါ solids များကို ဖန်တီးနိုင်သည်။ ထို့အပြင် [Cube](Part_Box.md), [Cylinder](Part_Cylinder.md) စသည့် အခြေခံ primitive solids များကိုလည်း ဖန်တီးနိုင်သည်။ ဤ objects များကို [Boolean operations](Part_Boolean.md) များဖြင့် ပေါင်းစည်း၍ ပိုစိတ်ရှုပ်ထွေးသော solids များ ဖန်တီးနိုင်ပါသည်။

The Part Workbench can also create objects that are not solids, such as faces, shells, and objects with only edges or vertices. It also provides a variety of general purpose tools for geometry manipulation, geometry validation, and making copies.

Part Workbench သည် မူလ စိုလ်ဓုတိ(သံ)မဟုတ်သော objects (ဥပမာ faces, shells, သို့မဟုတ် edge/vertex ပင်သာပါသော objects) များကိုလည်း ဖန်တီးနိုင်သည်။ ထို့အပြင် ဂျီယိုမက်ထရီကို ကိုင်တွယ်ခြင်း၊ ဂျီယိုမက်ထရီ စစ်ဆေးခြင်းနှင့် မိတ္တူများ ဖန်တီးရန် အသုံးများသော ကိရိယာအမျိုးမျိုးကို လည်း ပံ့ပိုးပေးသည်။

The <img alt="" src=images/Workbench_PartDesign.svg  style="width:16px;"> [PartDesign Workbench](PartDesign_Workbench.md) uses an alternative workflow for creating solids. For a detailed discussion of the Part Workbench versus the Part Design Workbench see [Part and Part Design](Part_and_PartDesign.md).

<img alt="" src=images/Workbench_PartDesign.svg  style="width:16px;"> [PartDesign Workbench](PartDesign_Workbench.md) (အစိတ်အပိုင်း ဒီဇိုင်း) သည် solids ဖန်တီးရာတွင် မတူကွဲပြားသော workflow တစ်မျိုးကို အသုံးပြုသည်။ Part Workbench နှင့် PartDesign Workbench တို့၏ ကွာခြားချက်များအကြောင်းကို ပိုမိုအသေးစိတ် သိလိုပါက [Part and Part Design](Part_and_PartDesign.md) ကို ကြည့်ပါ။

 ![](images/Part_Workbench_Example.jpg ) 

## Tools

### Solids toolbar 

-   <img alt="" src=images/Part_Box.svg  style="width:32px;"> [Box](Part_Box.md): Creates a box.

    -   <img alt="" src=images/Part_Box.svg  style="width:32px;"> [Box](Part_Box.md): ဘောက်စ် (box) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Cylinder.svg  style="width:32px;"> [Cylinder](Part_Cylinder.md): Creates a cylinder.

    -   <img alt="" src=images/Part_Cylinder.svg  style="width:32px;"> [Cylinder](Part_Cylinder.md): ဆိုင်ကလိန် (cylinder) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Sphere.svg  style="width:32px;"> [Sphere](Part_Sphere.md): Creates a sphere.

    -   <img alt="" src=images/Part_Sphere.svg  style="width:32px;"> [Sphere](Part_Sphere.md): ဘောလုံးပုံ (sphere) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Cone.svg  style="width:32px;"> [Cone](Part_Cone.md): Creates a cone.

    -   <img alt="" src=images/Part_Cone.svg  style="width:32px;"> [Cone](Part_Cone.md): ကိုန်ပုံ (cone) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Torus.svg  style="width:32px;"> [Torus](Part_Torus.md): Creates a torus.

    -   <img alt="" src=images/Part_Torus.svg  style="width:32px;"> [Torus](Part_Torus.md): တိုရပ်စ် (torus) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Tube.svg  style="width:32px;"> [Tube](Part_Tube.md): Creates a tube.

    -   <img alt="" src=images/Part_Tube.svg  style="width:32px;"> [Tube](Part_Tube.md): တိုက် (tube) ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Primitives.svg  style="width:32px;"> [Create primitives\...](Part_Primitives.md): A tool to create one of the following primitives:

  - <img alt="" src=images/Part_Plane.svg  style="width:32px;"> [Plane](Part_Plane.md): Creates a plane.

    - <img alt="" src=images/Part_Plane.svg  style="width:32px;"> [Plane](Part_Plane.md): မျက်နှာပြင် (plane) ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Box.svg  style="width:32px;"> [Box](Part_Box.md): Creates a box. This object can also be created with the [Box](Part_Box.md) tool.

    - <img alt="" src=images/Part_Box.svg  style="width:32px;"> [Box](Part_Box.md): ဘောက်စ်ကို ဖန်တီးသည်။ ဤ object ကို [Box](Part_Box.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Cylinder.svg  style="width:32px;"> [Cylinder](Part_Cylinder.md): Creates a cylinder. This object can also be created with the [Cylinder](Part_Cylinder.md) tool.

    - <img alt="" src=images/Part_Cylinder.svg  style="width:32px;"> [Cylinder](Part_Cylinder.md): ဆိုင်ကလိန်ကို ဖန်တီးသည်။ ဤ object ကို [Cylinder](Part_Cylinder.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Cone.svg  style="width:32px;"> [Cone](Part_Cone.md): Creates a cone. This object can also be created with the [Cone](Part_Cone.md) tool.

    - <img alt="" src=images/Part_Cone.svg  style="width:32px;"> [Cone](Part_Cone.md): ကိုန်ကို ဖန်တီးသည်။ ဤ object ကို [Cone](Part_Cone.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Sphere.svg  style="width:32px;"> [Sphere](Part_Sphere.md): Creates a sphere. This object can also be created with the [Sphere](Part_Sphere.md) tool.

    - <img alt="" src=images/Part_Sphere.svg  style="width:32px;"> [Sphere](Part_Sphere.md): sphere ကို ဖန်တီးသည်။ [Sphere](Part_Sphere.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Ellipsoid.svg  style="width:32px;"> [Ellipsoid](Part_Ellipsoid.md): Creates a ellipsoid.

    - <img alt="" src=images/Part_Ellipsoid.svg  style="width:32px;"> [Ellipsoid](Part_Ellipsoid.md): ellipsoid ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Torus.svg  style="width:32px;"> [Torus](Part_Torus.md): Creates a torus. This object can also be created with the [Torus](Part_Torus.md) tool.

    - <img alt="" src=images/Part_Torus.svg  style="width:32px;"> [Torus](Part_Torus.md): torus ကို ဖန်တီးသည်။ [Torus](Part_Torus.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Prism.svg  style="width:32px;"> [Prism](Part_Prism.md): Creates a prism.

    - <img alt="" src=images/Part_Prism.svg  style="width:32px;"> [Prism](Part_Prism.md): prism ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Wedge.svg  style="width:32px;"> [Wedge](Part_Wedge.md): Creates a wedge.

    - <img alt="" src=images/Part_Wedge.svg  style="width:32px;"> [Wedge](Part_Wedge.md): wedge ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Helix.svg  style="width:32px;"> [Helix](Part_Helix.md): Creates a helix.

    - <img alt="" src=images/Part_Helix.svg  style="width:32px;"> [Helix](Part_Helix.md): helix ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Spiral.svg  style="width:32px;"> [Spiral](Part_Spiral.md): Creates a spiral.

    - <img alt="" src=images/Part_Spiral.svg  style="width:32px;"> [Spiral](Part_Spiral.md): spiral ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Circle.svg  style="width:32px;"> [Circle](Part_Circle.md): Creates a circular arc.

    - <img alt="" src=images/Part_Circle.svg  style="width:32px;"> [Circle](Part_Circle.md): ဝန်းရိုးအာကာ (circular arc) ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Ellipse.svg  style="width:32px;"> [Ellipse](Part_Ellipse.md): Creates an elliptical arc.

    - <img alt="" src=images/Part_Ellipse.svg  style="width:32px;"> [Ellipse](Part_Ellipse.md): အသားချော အပျော့ပုံ (elliptical arc) ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Point.svg  style="width:32px;"> [Point](Part_Point.md): Creates a point.

    - <img alt="" src=images/Part_Point.svg  style="width:32px;"> [Point](Part_Point.md): အချက် (point) ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_Line.svg  style="width:32px;"> [Line](Part_Line.md): Creates a line.

    - <img alt="" src=images/Part_Line.svg  style="width:32px;"> [Line](Part_Line.md): တန်း (line) ကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_RegularPolygon.svg  style="width:32px;"> [Regular polygon](Part_RegularPolygon.md): Creates a regular polygon.

    - <img alt="" src=images/Part_RegularPolygon.svg  style="width:32px;"> [Regular polygon](Part_RegularPolygon.md): စံနမူနာ polygon ကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Builder.svg  style="width:32px;"> [Shape builder\...](Part_Builder.md): Creates shapes from various primitives.

    -   <img alt="" src=images/Part_Builder.svg  style="width:32px;"> [Shape builder\...](Part_Builder.md): မတူညီသော primitives များမှ shapes များကို ဖန်တီးပေးသည်။

### Part tools toolbar 

-   <img alt="" src=images/Sketcher_NewSketch.svg  style="width:32px;"> [Create sketch](Sketcher_NewSketch.md): Creates a new sketch and opens the [Sketcher Dialog](Sketcher_Dialog.md) to edit it.

    -   <img alt="" src=images/Sketcher_NewSketch.svg  style="width:32px;"> [Create sketch](Sketcher_NewSketch.md): စကစ် အသစ်တစ်ခုကို ဖန်တီးပြီး ပြန်ပြင်ရန် [Sketcher Dialog](Sketcher_Dialog.md) ကို ဖွင့်ပေးသည်။ (Sketcher — ပုံကြမ်းဖန်တီးမှု / စကစ်)

-   <img alt="" src=images/Part_Extrude.svg  style="width:32px;"> [Extrude](Part_Extrude.md): Extrudes planar faces.

    -   <img alt="" src=images/Part_Extrude.svg  style="width:32px;"> [Extrude](Part_Extrude.md): ပလန်းမျက်နှာပြင်များကို အထွာထုတ်၍ စိုလ်ဓုတိ (solid) အဖြစ် ပြောင်းလဲသည် (Extrude / ပြားချပ်ပိုင်းဖန်တီးခြင်း)။

-   <img alt="" src=images/Part_Revolve.svg  style="width:32px;"> [Revolve](Part_Revolve.md): Creates a solid by revolving an object (not a solid) around an axis.

    -   <img alt="" src=images/Part_Revolve.svg  style="width:32px;"> [Revolve](Part_Revolve.md): အရာဝတ္ထုတစ်ခု (solid မဟုတ်သော) ကို အတိုင်းအလျှောက်လှည့်၍ solid ဖန်တီးပေးသည်။ (Revolve)

-   <img alt="" src=images/Part_Mirror.svg  style="width:32px;"> [Mirror](Part_Mirror.md): Mirrors the selected object across a mirror plane.

    -   <img alt="" src=images/Part_Mirror.svg  style="width:32px;"> [Mirror](Part_Mirror.md): mirror plane ကို အခြေခံ၍ ရွေးထားသော object ကို ကရက်ရှင်း (mirror) ပြုလုပ်သည်။

-   <img alt="" src=images/Part_Scale.svg  style="width:32px;"> [Scale](Part_Scale.md): Scales one or more shapes. <small>(v1.0)</small> 

    -   <img alt="" src=images/Part_Scale.svg  style="width:32px;"> [Scale](Part_Scale.md): shape (တစ်ခု သို့မဟုတ် တစ်ချို့) များကို အရွယ်အစား ပြောင်းသည်။ <small>(v1.0)</small>

-   <img alt="" src=images/Part_Fillet.svg  style="width:32px;"> [Fillet](Part_Fillet.md): Fillets (rounds) edges of an object.

    -   <img alt="" src=images/Part_Fillet.svg  style="width:32px;"> [Fillet](Part_Fillet.md): object ၏ အနားများကို စကွက်စကာ (round) အဖြစ် ဖန်တီးပေးသည် (Fillet)။

-   <img alt="" src=images/Part_Chamfer.svg  style="width:32px;"> [Chamfer](Part_Chamfer.md): Chamfers edges of an object.

    -   <img alt="" src=images/Part_Chamfer.svg  style="width:32px;"> [Chamfer](Part_Chamfer.md): object ၏ အနားများကို chamfer ပြုလုပ်သည်။

-   <img alt="" src=images/Part_MakeFace.svg  style="width:32px;"> [Make face from wires](Part_MakeFace.md): Makes a face from a set of wires (contours).

    -   <img alt="" src=images/Part_MakeFace.svg  style="width:32px;"> [Make face from wires](Part_MakeFace.md): wire (contour) များအစုံမှ မျက်နှာပြင် (face) တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_RuledSurface.svg  style="width:32px;"> [Ruled Surface](Part_RuledSurface.md): Creates a ruled surface.

    -   <img alt="" src=images/Part_RuledSurface.svg  style="width:32px;"> [Ruled Surface](Part_RuledSurface.md): ruled surface တစ်မျိုးကို ဖန်တီးသည်။

-   <img alt="" src=images/Part_Loft.svg  style="width:32px;"> [Loft](Part_Loft.md): Lofts from one profile to another.

    -   <img alt="" src=images/Part_Loft.svg  style="width:32px;"> [Loft](Part_Loft.md): ပရိုဖိုင်တစ်ခုမှ တစ်ခုသို့ loft ဖန်တီးသည်။

-   <img alt="" src=images/Part_Sweep.svg  style="width:32px;"> [Sweep](Part_Sweep.md): Sweeps one or more profiles along a path.

    -   <img alt="" src=images/Part_Sweep.svg  style="width:32px;"> [Sweep](Part_Sweep.md): လမ်းကြောင်းတစ်ခုအပေါ် ပရိုဖိုင် တစ်ခု (သို့) များစွာကို sweep ပြုလုပ်သည်။

-   <img alt="" src=images/Part_Section.svg  style="width:32px;"> [Section](Part_Section.md): Creates a section by intersecting an object with a section plane.

    -   <img alt="" src=images/Part_Section.svg  style="width:32px;"> [Section](Part_Section.md): section plane ဖြင့် အရာဝတ္ထုကို ထိပ်တိုက်ဖြတ်၍ section တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_CrossSections.svg  style="width:32px;"> [Cross sections\...](Part_CrossSections.md): Creates one or more cross-sections through an object.

    -   <img alt="" src=images/Part_CrossSections.svg  style="width:32px;"> [Cross sections\...](Part_CrossSections.md): object ကို ဖြတ်၍ တစ်ခု (သို့) အများအပြား cross-section များ ဖန်တီးသည်။

-   <img alt="" src=images/Part_Offset.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Offset:

  - <img alt="" src=images/Part_Offset.svg  style="width:32px;"> [3D Offset](Part_Offset.md): Constructs a parallel shape at a certain distance from an original.

    - <img alt="" src=images/Part_Offset.svg  style="width:32px;"> [3D Offset](Part_Offset.md): မူရင်း shape ထံမှ သတ်မှတ်ထားသော အကွာအဝေးပမာဏအတိုင်း ပေါ်လွင်သော parallel shape ကို တည်ဆောက်သည်။

  - <img alt="" src=images/Part_Offset2D.svg  style="width:32px;"> [2D Offset](Part_Offset2D.md): Constructs a parallel wire at certain distance from an original, or enlarges/shrinks a planar face.

    - <img alt="" src=images/Part_Offset2D.svg  style="width:32px;"> [2D Offset](Part_Offset2D.md): မူရင်း wire ထံမှ သတ်မှတ်ထားသော အကွာအဝေးပမာဏအတိုင်း parallel wire တစ်ခု တည်ဆောက်သည်၊ သို့မဟုတ် planar face ကို တိုး/ချုံး ပြုလုပ်သည်။

-   <img alt="" src=images/Part_Thickness.svg  style="width:32px;"> [Thickness](Part_Thickness.md): Hollows out a solid.

    -   <img alt="" src=images/Part_Thickness.svg  style="width:32px;"> [Thickness](Part_Thickness.md): solid အား ဗလာအတွင်းအသွင် (hollow) ပြုလုပ်သည်။

-   <img alt="" src=images/Part_ProjectionOnSurface.svg  style="width:32px;"> [Projection on surface](Part_ProjectionOnSurface.md): Projects a logo, text or any face, wire or edge onto a surface.

    -   <img alt="" src=images/Part_ProjectionOnSurface.svg  style="width:32px;"> [Projection on surface](Part_ProjectionOnSurface.md): logo, စာသား သို့မဟုတ် face, wire, edge များကို မျက်နှာပြင်ပေါ်သို့ projection ပြုလုပ်သည်။

-   <img alt="" src=images/Part_ColorPerFace.svg  style="width:32px;"> [Color per face](Part_ColorPerFace.md): Assigns colors to individual faces of objects.

    -   <img alt="" src=images/Part_ColorPerFace.svg  style="width:32px;"> [Color per face](Part_ColorPerFace.md): object ၏ မျက်နှာပြင် တစ်ခုချင်းစီအား အရောင်သတ်မှတ်ပေးသည်။

### Boolean toolbar 

-   <img alt="" src=images/Part_Compound.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Compound:

  - <img alt="" src=images/Part_Compound.svg  style="width:32px;"> [Make compound](Part_Compound.md): Creates a compound from the selected objects.

    - <img alt="" src=images/Part_Compound.svg  style="width:32px;"> [Make compound](Part_Compound.md): ရွေးထားသော objects များမှ compound တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_ExplodeCompound.svg  style="width:32px;"> [Explode compound](Part_ExplodeCompound.md): Splits up compounds.

    - <img alt="" src=images/Part_ExplodeCompound.svg  style="width:32px;"> [Explode compound](Part_ExplodeCompound.md): compound ကို အစိတ်အပိုင်းများခွဲထုတ်သည်။

  - <img alt="" src=images/Part_CompoundFilter.svg  style="width:32px;"> [Compound Filter](Part_CompoundFilter.md): Extracts the individual pieces from compounds.

    - <img alt="" src=images/Part_CompoundFilter.svg  style="width:32px;"> [Compound Filter](Part_CompoundFilter.md): compound များထဲမှ တစ်ခုချင်းစီ အပိုင်းအစများကို ဆွဲထုတ်ပေးသည်။

-   <img alt="" src=images/Part_Boolean.svg  style="width:32px;"> [Boolean](Part_Boolean.md): Performs boolean operations on two objects.

    -   <img alt="" src=images/Part_Boolean.svg  style="width:32px;"> [Boolean](Part_Boolean.md): အရာဝတ္ထုနှစ်ခုအပေါ် boolean ကိရိယာများကို လုပ်ဆောင်သည်။

-   <img alt="" src=images/Part_Cut.svg  style="width:32px;"> [Cut](Part_Cut.md): Cuts one object from another.

    -   <img alt="" src=images/Part_Cut.svg  style="width:32px;"> [Cut](Part_Cut.md): တစ်ခုသော object ကို အခြား object ထဲမှ ဖြုတ်ထုတ်သည် (cut)။

-   <img alt="" src=images/Part_Fuse.svg  style="width:32px;"> [Union](Part_Fuse.md): Fuses two or more objects.

    -   <img alt="" src=images/Part_Fuse.svg  style="width:32px;"> [Union](Part_Fuse.md): object နှစ်ခု (သို့) ပိုများကို ဖျူးပေါင်း (fuse) ပြုလုပ်သည်။

-   <img alt="" src=images/Part_Common.svg  style="width:32px;"> [Intersection](Part_Common.md): Extracts the common part of two objects.

    -   <img alt="" src=images/Part_Common.svg  style="width:32px;"> [Intersection](Part_Common.md): object နှစ်ခုတွင် ရှိသော အနက်အစိတ်အပိုင်းကို ဆွဲထုတ်သည်။

-   <img alt="" src=images/Part_JoinConnect.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Join:

  - <img alt="" src=images/Part_JoinConnect.svg  style="width:32px;"> [Connect objects](Part_JoinConnect.md): Connects interiors of walled objects.

    - <img alt="" src=images/Part_JoinConnect.svg  style="width:32px;"> [Connect objects](Part_JoinConnect.md): ဝေါဟာရရှိသော objects ၏ အတွင်းပိုင်းများကို ဆက်သွယ်ပေးသည်။

  - <img alt="" src=images/Part_JoinEmbed.svg  style="width:32px;"> [Embed object](Part_JoinEmbed.md): Embeds a walled object into another walled object.

    - <img alt="" src=images/Part_JoinEmbed.svg  style="width:32px;"> [Embed object](Part_JoinEmbed.md): ဝေါဟာရရှိ object တစ်ခုကို အခြားဝေါဟာရ object အတွင်း သွင်းဆောင်သည်။

  - <img alt="" src=images/Part_JoinCutout.svg  style="width:32px;"> [Cutout for object](Part_JoinCutout.md): Creates a cutout in a wall of an object for another walled object.

    - <img alt="" src=images/Part_JoinCutout.svg  style="width:32px;"> [Cutout for object](Part_JoinCutout.md): ဝေါဟာရ object တစ်ခုအတွက် အခြားဝေါဟာရ object ထည့်ရန် မျက်နှာကျက်တွင် cutout တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_BooleanFragments.svg  style="width:" height="32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> Split:

  - <img alt="" src=images/Part_BooleanFragments.svg  style="width:32px;"> [Boolean fragments](Part_BooleanFragments.md): Creates all pieces obtained from Boolean operations.

    - <img alt="" src=images/Part_BooleanFragments.svg  style="width:32px;"> [Boolean fragments](Part_BooleanFragments.md): Boolean လုပ်ငန်းစဉ်များမှ ထွက်လာသော အပိုင်းအစများအားလုံးကို ဖန်တီးပေးသည်။

  - <img alt="" src=images/Part_SliceApart.svg  style="width:32px;"> [Slice apart](Part_SliceApart.md): Slices and splits an object by intersecting it with other objects.

    - <img alt="" src=images/Part_SliceApart.svg  style="width:32px;"> [Slice apart](Part_SliceApart.md): အခြား objects များနှင့် တပ်ဆက်ကျော်ဖြတ်၍ object ကို ဖြတ်တိုက် ခွဲထုတ်သည်။

  - <img alt="" src=images/Part_Slice.svg  style="width:32px;"> [Slice to compound](Part_Slice.md): Slices an object by intersecting it with other objects.

    - <img alt="" src=images/Part_Slice.svg  style="width:32px;"> [Slice to compound](Part_Slice.md): အခြား objects များနှင့် တွက်ရောက်တပ်ဆက်၍ object ကို slice လုပ်ကာ compound ပြုလုပ်သည်။

  - <img alt="" src=images/Part_XOR.svg  style="width:32px;"> [Boolean XOR](Part_XOR.md): Removes space shared by an even number of objects.

    - <img alt="" src=images/Part_XOR.svg  style="width:32px;"> [Boolean XOR](Part_XOR.md): အရေအတွက် စုံညီသော objects များ အစိတ်အပိုင်းမျှဝေထားသော နေရာများကို ဖယ်ရှားသည်။

-   <img alt="" src=images/Part_CheckGeometry.svg  style="width:32px;"> [Check geometry](Part_CheckGeometry.md): Checks the geometry of selected objects for errors.

    - <img alt="" src=images/Part_CheckGeometry.svg  style="width:32px;"> [Check geometry](Part_CheckGeometry.md): ရွေးထားသော objects များ၏ ဂျီယိုမက်ထရီကို အမွားများရှိ/မရှိ စစ်ဆေးသည်။

-   <img alt="" src=images/Part_Defeaturing.svg  style="width:32px;"> [Defeaturing](Part_Defeaturing.md): Removes features from an object.

    - <img alt="" src=images/Part_Defeaturing.svg  style="width:32px;"> [Defeaturing](Part_Defeaturing.md): object မှ မလိုအပ်သည့် features များကို ဖယ်ရှားသည်။

### Other tools 

-   <img alt="" src=images/Part_Import.svg  style="width:32px;"> [Import CAD file\...](Part_Import.md): Imports from \*.IGES, \*.STEP, or \*.BREP files.

    -   <img alt="" src=images/Part_Import.svg  style="width:32px;"> [Import CAD file\...](Part_Import.md): \*.IGES, \*.STEP၊ \*.BREP ဖိုင်များမှ ထည့်သွင်းသည်။

-   <img alt="" src=images/Part_Export.svg  style="width:32px;"> [Export CAD file\...](Part_Export.md): Exports to \*.IGES, \*.STEP, or \*.BREP files.

    -   <img alt="" src=images/Part_Export.svg  style="width:32px;"> [Export CAD file\...](Part_Export.md): \*.IGES, \*.STEP၊ \*.BREP ဖိုင်များသို့ ထုတ်ယူပေးသည်။

-   <img alt="" src=images/Part_BoxSelection.svg  style="width:32px;"> [Box selection](Part_BoxSelection.md): Selects faces from a rectangular area.

    -   <img alt="" src=images/Part_BoxSelection.svg  style="width:32px;"> [Box selection](Part_BoxSelection.md): စတုရန်း/ထောင့်ပုံအကွာအဝေးကနေ မျက်နှာပြင်များကို ရွေးချယ်ပေးသည်။

-   <img alt="" src=images/Part_ShapeFromMesh.svg  style="width:32px;"> [Create shape from mesh](Part_ShapeFromMesh.md): Creates shapes from mesh objects.

    -   <img alt="" src=images/Part_ShapeFromMesh.svg  style="width:32px;"> [Create shape from mesh](Part_ShapeFromMesh.md): mesh objects များမှ shape များ ဖန်တီးပေးသည်။

-   <img alt="" src=images/Part_PointsFromMesh.svg  style="width:32px;"> [Create points object from geometry](Part_PointsFromMesh.md): Creates points objects from geometric objects.

    -   <img alt="" src=images/Part_PointsFromMesh.svg  style="width:32px;"> [Create points object from geometry](Part_PointsFromMesh.md): ဂျီယိုမက်ထရီအခြေခံ object များမှ point object များ ဖန်တီးပေးသည်။

-   <img alt="" src=images/Part_MakeSolid.svg  style="width:32px;"> [Convert to solid](Part_MakeSolid.md): Creates solids from shape objects.

    -   <img alt="" src=images/Part_MakeSolid.svg  style="width:32px;"> [Convert to solid](Part_MakeSolid.md): shape object များကို solid အဖြစ် ပြောင်းလဲဖန်တီးသည်။

-   <img alt="" src=images/Part_ReverseShape.svg  style="width:32px;"> [Reverse shapes](Part_ReverseShape.md): Creates parametric copies with reversed face normals from selected objects.

    -   <img alt="" src=images/Part_ReverseShape.svg  style="width:32px;"> [Reverse shapes](Part_ReverseShape.md): ရွေးထားသော objects များမှ face normals ကို ပြန်လည်လှမ်းထားသော parametric မိတ္တူများကို ဖန်တီးပေးသည်။

-   Create a copy:

  - <img alt="" src=images/Part_SimpleCopy.svg  style="width:32px;"> [Create simple copy](Part_SimpleCopy.md): Creates non-parametric copies of objects.

    - <img alt="" src=images/Part_SimpleCopy.svg  style="width:32px;"> [Create simple copy](Part_SimpleCopy.md): object များ၏ non-parametric မိတ္တူများကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_TransformedCopy.svg  style="width:32px;"> [Create transformed copy](Part_TransformedCopy.md): Creates non-parametric copies of objects. It is intended for objects nested in containers.

    - <img alt="" src=images/Part_TransformedCopy.svg  style="width:32px;"> [Create transformed copy](Part_TransformedCopy.md): object များ၏ non-parametric မိတ္တူများကို ဖန်တီးသည်။ ဤကိရိယာကို container အတွင်း nested ဖြစ်သော objects များအတွက် သတ်မှတ်ထားသည်။

  - <img alt="" src=images/Part_ElementCopy.svg  style="width:32px;"> [Create shape element copy](Part_ElementCopy.md): Creates non-parametric copies of subelements: vertices, edges and faces.

    - <img alt="" src=images/Part_ElementCopy.svg  style="width:32px;"> [Create shape element copy](Part_ElementCopy.md): vertices, edges, faces စသည့် subelements များ၏ non-parametric မိတ္တူများကို ဖန်တီးသည်။

  - <img alt="" src=images/Part_RefineShape.svg  style="width:32px;"> [Refine shape](Part_RefineShape.md): Creates parametric copies with a refined shape from selected objects. It removes unnecessary edges from planar and cylindrical faces.

    - <img alt="" src=images/Part_RefineShape.svg  style="width:32px;"> [Refine shape](Part_RefineShape.md): ရွေးထားသော objects များမှ ကိုးကားထား၍ refined shape ပါသော parametric မိတ္တူများကို ဖန်တီးသည်။ planar နှင့် cylindrical မျက်နှာပြင်များမှ မလိုအပ်သော အနားများကို ဖယ်ရှားပေးသည်။

-   <img alt="" src=images/Part_EditAttachment.svg  style="width:32px;"> [Attachment\...](Part_EditAttachment.md): Attaches an object to one or more other objects.

    -   <img alt="" src=images/Part_EditAttachment.svg  style="width:32px;"> [Attachment\...](Part_EditAttachment.md): object တစ်ခုကို (သို့) ပိုများသော အခြား object များသို့ attachment ဖြင့် တွဲဆက်ပေးသည်။

## Obsolete tools 

### Measure

The <img alt="" src=images/Std_Measure.svg  style="width:32px;"> [Std Measure](Std_Measure.md) tool replaces the tools listed below. <small>(v1.0)</small> 

<img alt="" src=images/Std_Measure.svg  style="width:32px;"> [Std Measure](Std_Measure.md) ကိရိယာသည် အောက်တွင် ဖော်ပြထားသော ကိရိယာများအား အစားထိုးပေးသည်။ <small>(v1.0)</small>

-   <img alt="" src=images/Part_Measure_Linear.svg  style="width:32px;"> [Measure Linear](Part_Measure_Linear.md): Creates a linear measurement. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Linear.svg  style="width:32px;"> [Measure Linear](Part_Measure_Linear.md): ရိုးလိုင်းတိုင်းတာမှု (linear measurement) တစ်ခုကို ဖန်တီးသည်။ <small>(v1.0 မှာ မရှိ)</small>

-   <img alt="" src=images/Part_Measure_Angular.svg  style="width:32px;"> [Measure Angular](Part_Measure_Angular.md): Creates an angular measurement. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Angular.svg  style="width:32px;"> [Measure Angular](Part_Measure_Angular.md): ဘောလုံးအနားတိုင်းတာမှု (angular measurement) တစ်ခုကို ဖန်တီးသည်။ <small>(v1.0 မှာ မရှိ)</small>

-   <img alt="" src=images/Part_Measure_Refresh.svg  style="width:32px;"> [Measure Refresh](Part_Measure_Refresh.md): Updates all measurements. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Refresh.svg  style="width:32px;"> [Measure Refresh](Part_Measure_Refresh.md): တိုင်းတာမှုများအားလုံးကို အပ်ဒိတ်လုပ်ပေးသည်။ <small>(v1.0 မှာ မရှိ)</small>

-   <img alt="" src=images/Part_Measure_Clear_All.svg  style="width:32px;"> [Clear All](Part_Measure_Clear_All.md) and [View Measure Clear All](View_Measure_Clear_All.md): Clears all measurements. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Clear_All.svg  style="width:32px;"> [Clear All](Part_Measure_Clear_All.md) and [View Measure Clear All](View_Measure_Clear_All.md): များစွာသော တိုင်းတာချက်များအားလုံးကို ဖျက်သိမ်းပေးသည်။ <small>(v1.0 မှာ မရှိ)</small>

-   <img alt="" src=images/Part_Measure_Toggle_All.svg  style="width:32px;"> [Toggle All](Part_Measure_Toggle_All.md) and [View Measure Toggle All](View_Measure_Toggle_All.md): Shows or hides all measurements. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Toggle_All.svg  style="width:32px;"> [Toggle All](Part_Measure_Toggle_All.md) and [View Measure Toggle All](View_Measure_Toggle_All.md): တိုင်းတာချက်များအားလုံးကို ပြသ/ဖျောက် ပြုလုပ်နိုင်သည်။ <small>(v1.0 မှာ မရှိ)</small>

-   <img alt="" src=images/Part_Measure_Toggle_3D.svg  style="width:32px;"> [Toggle 3D](Part_Measure_Toggle_3D.md): Shows or hides 3D measurements. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Toggle_3D.svg  style="width:32px;"> [Toggle 3D](Part_Measure_Toggle_3D.md): 3D တိုင်းတာချက်များကို ပြသ/ဖျောက် ပြုလုပ်သည်။ <small>(v1.0 မှာ မရှိ)</small>

-   <img alt="" src=images/Part_Measure_Toggle_Delta.svg  style="width:32px;"> [Toggle Delta](Part_Measure_Toggle_Delta.md): Shows or hides delta measurements. Not available in <small>(v1.0)</small> .

    -   <img alt="" src=images/Part_Measure_Toggle_Delta.svg  style="width:32px;"> [Toggle Delta](Part_Measure_Toggle_Delta.md): delta တိုင်းတာချက်များကို ပြသ/ဖျောက် ပြုလုပ်သည်။ <small>(v1.0 မှာ မရှိ)</small>

## Preferences

-   <img alt="" src=images/Preferences-part_design.svg  style="width:32px;"> [Preferences](PartDesign_Preferences.md): Preferences for the Part Workbench.
-   <img alt="" src=images/Preferences-import-export.svg  style="width:32px;"> [Import Export Preferences](Import_Export_Preferences.md): Preferences for importing from and exporting to different file formats.
-   [Fine-tuning](Fine-tuning#Part_Workbench.md): Some extra parameters to fine-tune Part behavior.

-   <img alt="" src=images/Preferences-part_design.svg  style="width:32px;"> [Preferences](PartDesign_Preferences.md): Part Workbench (လုပ်ငန်းခွင်) အတွက် ဆက်တင်များ။
-   <img alt="" src=images/Preferences-import-export.svg  style="width:32px;"> [Import Export Preferences](Import_Export_Preferences.md): ဖိုင်ဖော်แมတ်အမျိုးမျိုးမှ ထည့်သွင်းခြင်းနှင့် ထုတ်ယူခြင်းတို့အတွက် Preference များ။
-   [Fine-tuning](Fine-tuning#Part_Workbench.md): Part ၏ ဖန်တီးမှုနှင့် အပြုအမူကို ထိန်းသိမ်းရန် အပို parameter များ။

## Scripting

See [Part scripting](Part_scripting.md).

## Tutorials

-   [Import from STL or OBJ](Import_from_STL_or_OBJ.md): How to import STL/OBJ files in FreeCAD
-   [Export to STL or OBJ](Export_to_STL_or_OBJ.md): How to export STL/OBJ files from FreeCAD
-   [Whiffle Ball tutorial](Whiffle_Ball_tutorial.md): How to use the Part Workbench

-   [Import from STL or OBJ](Import_from_STL_or_OBJ.md): FreeCAD (ဖရီးကက် (FreeCAD)) တွင် STL/OBJ ဖိုင်များကို မည်သို့ import ချするか (ဘယ်လိုလုပ်မည်)
-   [Export to STL or OBJ](Export_to_STL_or_OBJ.md): FreeCAD မှ STL/OBJ ဖိုင်များကို မည်သို့ export ချするか (ဘယ်လိုလုပ်မည်)
-   [Whiffle Ball tutorial](Whiffle_Ball_tutorial.md): Part Workbench (လုပ်ငန်းခွင်) ကို မည်သို့ အသုံးပြုမည်ကို ရှင်းလင်းသင်ကြားချက်

---
⏵ [documentation index](../README.md) > [Workbenches](Category_Workbenches.md) > [Part](Category_Part.md) > Part Workbench (လုပ်ငန်းခွင်)