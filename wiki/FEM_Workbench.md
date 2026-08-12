# <img alt="FEM workbench icon" src=images/Workbench_FEM.svg  style="width:64px;"> FEM လုပ်ငန်းခွင် (FEM Workbench)

 

## နိဒါန်း

The [FEM Workbench](FEM_Workbench.md) သည် ဖရီးကက် (FreeCAD) အတွက် ခေတ်မီသော [finite element analysis](https://en.wikipedia.org/wiki/Finite_element_analysis) (FEA / အပိုင်းငယ် စစ်ဆေးခြင်း) လုပ်ငန်းစဉ်ကို ပံ့ပိုးပေးသည်။ အဓိကအားဖြင့် ၎င်းသည် စစ်ဆေးမှုတစ်ခုအား ပြုလုပ်ရန် လိုအပ်သော ကိရိယာများအားလုံးကို တစ်ခုတည်းသော graphical user interface (GUI) အတွင်း ပေါင်းစည်းထားခြင်းကို ဆိုလိုသည်။

 <img alt="" src=images/FemWorkbench.jpg  style="width:300px;"> 

## လုပ်ငန်းစဉ်

Finite element analysis ကို ဆောင်ရွက်ရန် လိုအပ်သော အဆင့်များမှာ -

1.  Preprocessing: စစ်ဆေးမှု ပြဿနာကို ပြင်ဆင်ခြင်း။
    1.  Modeling the geometry: ဖရီးကက် (FreeCAD) ဖြင့် ဂျီယိုမက်ထရီ (geometry) ကို ဖန်တီးခြင်း သို့မဟုတ် အခြား အပလီကေးရှင်းမှ တင်သွင်းခြင်း။
    2.  Creating an analysis: စစ်ဆေးမှု (analysis) တစ်ခု ဖန်တီးခြင်း။
        1.  ဂျီယိုမက်ထရီ မော်ဒယ်ပေါ်တွင် load များနှင့် fixed supports ကဲ့သို့သော ကန့်သတ်ချက်များ (Constraint) များကို ထည့်သွင်းခြင်း။
        2.  ဂျီယိုမက်ထရီ မော်ဒယ်၏ အစိတ်အပိုင်းများတွင် ပစ္စည်း (materials) များ ထည့်သွင်းခြင်း။
        3.  ဂျီယိုမက်ထရီ မော်ဒယ်အတွက် finite element mesh တစ်ခု ဖန်တီးခြင်း သို့မဟုတ် အခြား အပလီကေးရှင်းမှ mesh ကို တင်သွင်းခြင်း။
2.  Solving: ဖရီးကက် (FreeCAD) မှာ အပြင်ဘက် solver တစ်ခုကို အလုပ်ဖြစ်စေခြင်း။
3.  Postprocessing: ဖရီးကက် (FreeCAD) အတွင်းမှ စစ်ဆေးမှု ရလဒ်များကို မြင်တွေ့ပြသခြင်း သို့မဟုတ် အခြား အပလီကေးရှင်းဖြင့် နောက်ဆက်တွဲ ဆန်းစစ်နိုင်ရန် ရလဒ်များကို ပို့ခြင်း။

FEM Workbench ကို Linux, Windows, နှင့် Mac OSX ပေါ်တွင် အသုံးပြုနိုင်သည်။ workbench သည် အပြင်ဘက် solvers များကို အသုံးပြုသဖြင့်၊ လက်လုပ် စက်တင်ခြင်းများ၏ အပြည့်အဝ တာဝန်ယူမှုသည် သင်အသုံးပြုနေသော ကိုယ့် operating system အပေါ် မူတည်ပါသည်။ အပြင်ဘက် ကိရိယာများ သတ်မှတ်ရန် လမ်းညွှန်ချက်များအတွက် [FEM Install](FEM_Install.md) ကို ကြည့်ပါ။

 <img alt="" src=images/FEM_Workbench_workflow.svg  style="width:600px;"> 



*FEM Workbench ၏ လုပ်ငန်းစဉ်；workbench သည် အပြင်ဘက် အစီအစဉ် နှစ်ခုကို ခေါ်ဆောင်၍ တစ်စုံထု၏ meshing ကို ပြုလုပ်ပေးပြီး finite element ပြဿနာ၏ အဖြေကို ဆောင်ရွက်ပေးသည်။*

## Menu: Model 

-   <img alt="" src=images/FEM_Analysis.svg  style="width:32px;"> [Analysis container](FEM_Analysis.md): စက်မှုဆိုင်ရာ စစ်ဆေးမှု (mechanical analysis) အတွက် container အသစ်ကို ဖန်တီးသည်။ Tree view တွင် solid ကို ရွေးထားပြီး ဤအရာကို နှိပ်လျှင် meshing dialog သွားဖြစ်ပါမည်။

### ပစ္စည်းများ (Materials)

  - <img alt="" src=images/FEM_MaterialSolid.svg  style="width:32px;"> [Material for solid](FEM_MaterialSolid.md): ဒေတာဘေ့စ်မှ solid အတွက် ပစ္စည်းတစ်ခုကို ရွေးချယ်ရန် အခွင့်အလမ်းပေးသည်။

  - <img alt="" src=images/FEM_MaterialFluid.svg  style="width:32px;"> [Material for fluid](FEM_MaterialFluid.md): ဒေတာဘေ့စ်မှ fluid အတွက် ပစ္စည်းတစ်ခုကို ရွေးချယ်ရန် အခွင့်အလမ်းပေးသည်။

  - <img alt="" src=images/FEM_MaterialMechanicalNonlinear.svg  style="width:32px;"> [Nonlinear mechanical material](FEM_MaterialMechanicalNonlinear.md): nonlinear mechanical material မော်ဒယ်တစ်ခု ထည့်သွင်းနိုင်သည်။

  - <img alt="" src=images/FEM_MaterialReinforced.svg  style="width:32px;"> [Reinforced material (concrete)](FEM_MaterialReinforced.md): matrix နှင့် reinforcement ပါဝင်သည့် reinforced materials များကို ဒေတာဘေ့စ်မှ ရွေးချယ်နိုင်သည်။

  - <img alt="" src=images/FEM_MaterialEditor.svg  style="width:32px;"> [Material editor](FEM_MaterialEditor.md): material editor ကို ဖွင့်၍ ပစ္စည်းများကို အယ်ဒီတ်ပြင်ဆင်နိုင်သည်။

### အစိတ်အပိုင်း ဂျီယိုမက်ထရီ (Element Geometry) 

  - <img alt="" src=images/FEM_ElementGeometry1D.svg  style="width:32px;"> [Beam cross section](FEM_ElementGeometry1D.md): beam elements များအတွက် cross section များ သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ElementRotation1D.svg  style="width:32px;"> [Beam rotation](FEM_ElementRotation1D.md): beam elements ၏ cross section များကို ဖျော်လှန်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ElementGeometry2D.svg  style="width:32px;"> [Shell plate thickness](FEM_ElementGeometry2D.md): shell element များ၏ thickness ကို သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ElementFluid1D.svg  style="width:32px;"> [Fluid section for 1D flow](FEM_ElementFluid1D.md): pneumatic နှင့် hydraulic network များအတွက် fluid section element တည်ဆောက်ရာတွင် အသုံးပြုသည်။

### အလျှပ်စစ် မျက်နှာပိုင်း ကန့်သတ်ချက်များ (Electromagnetic boundary conditions) 

  - <img alt="" src=images/FEM_ConstraintElectrostaticPotential.svg  style="width:32px;"> [Electrostatic potential boundary condition](FEM_ConstraintElectrostaticPotential.md): electrostatic potential ကို သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintCurrentDensity.svg  style="width:32px;"> [Current density boundary condition](FEM_ConstraintCurrentDensity.md): current density ကို သတ်မှတ်ရန် အသုံးပြုသည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/FEM_ConstraintMagnetization.svg  style="width:32px;"> [Magnetization boundary condition](FEM_ConstraintMagnetization.md): magnetization ကို သတ်မှတ်ရန် အသုံးပြုသည်။ <small>(v0.21)</small> 

### ရေဖြတ် ဆိုင်ရာ ကန့်သတ်ချက်များ (Fluid boundary conditions) 

  - <img alt="" src=images/FEM_ConstraintInitialFlowVelocity.svg  style="width:32px;"> [Initial flow velocity condition](FEM_ConstraintInitialFlowVelocity.md): အရွေ့မြန်နှုန်းအစ ပြဿနာကို (volume) သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintInitialPressure.svg  style="width:32px;"> [Initial pressure condition](FEM_ConstraintInitialPressure.md): ကိုယ်ထည် (volume) အတွက် initial pressure ကို သတ်မှတ်ရန် အသုံးပြုသည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/FEM_ConstraintFlowVelocity.svg  style="width:32px;"> [Flow velocity boundary condition](FEM_ConstraintFlowVelocity.md): edge (2D) သို့ face (3D) ပေါ်တွင် flow velocity ကို boundary condition အဖြစ် သတ်မှတ်ရန် အသုံးပြုသည်။

### ဂျီယိုမက်ထရီဆိုင်ရာ ချန်ခြင်း လက္ခဏာများ (Geometrical analysis features) 

  - <img alt="" src=images/FEM_ConstraintPlaneRotation.svg  style="width:32px;"> [Plane multi-point constraint](FEM_ConstraintPlaneRotation.md): တည်နေရာ nodes များကို တူညီသော ညာဘက် စက်ဝိုင်း (plane) အတွင်း ထားရှိရန် constraint သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintSectionPrint.svg  style="width:32px;"> [Section print feature](FEM_ConstraintSectionPrint.md): မျက်နှာပေါ်သတ်မှတ်ထားသော output variables (forces နှင့် moments) များကို data ဖိုင်သို့ ထုတ်ပေးရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintTransform.svg  style="width:32px;"> [Local coordinate system](FEM_ConstraintTransform.md): မျက်နှာတစ်ခုတွင် transform constraint တစ်ခု သတ်မှတ်ရန် အသုံးပြုသည်။

### مکانিক ကန့်သတ်ချက်များနှင့် ပြောင်းလှည့်မှု (Mechanical boundary conditions and loads) 

  - <img alt="" src=images/FEM_ConstraintFixed.svg  style="width:32px;"> [Fixed boundary condition](FEM_ConstraintFixed.md): point/edge/face(များ) အပေါ် fixed constraint တစ်ခု သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintRigidBody.svg  style="width:32px;"> [Rigid body constraint](FEM_ConstraintRigidBody.md): CalculiX ရဲ့ rigid body constraint ကို အကောင်အထည်ဖော်ရန် အသုံးပြုသည်။ ၎င်းက ရွေးချယ်ထားသော ဂျီယိုမက်ထရီ အရာဝတ္ထု၏ nodes များ၏ 動きを user သတ်မှတ်ထားသော reference point ၏ 動き နှင့် ဆက်စပ်စေသည်။ <small>(v1.0)</small> 

  - <img alt="" src=images/FEM_ConstraintDisplacement.svg  style="width:32px;"> [Displacement boundary condition](FEM_ConstraintDisplacement.md): point/edge/face(များ) အပေါ် displacement constraint တစ်ခု သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintContact.svg  style="width:32px;"> [Contact constraint](FEM_ConstraintContact.md): နှစ်ဖက်မျက်နှာများအကြား contact constraint ကို သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintTie.svg  style="width:32px;"> [Tie constraint](FEM_ConstraintTie.md): နှစ်ဖက်မျက်နှာများအကြား tie constraint ("bonded contact") သို့မဟုတ် <small>(v1.0)</small>၊ cyclic symmetry ကို သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintSpring.svg  style="width:32px;"> [Spring](FEM_ConstraintSpring.md): spring တစ်ခုကို သတ်မှတ်ရန် အသုံးပြုသည်။ <small>(v0.20)</small> 

  - <img alt="" src=images/FEM_ConstraintForce.svg  style="width:32px;"> [Force load](FEM_ConstraintForce.md): [N] တန်ဖိုးဖြင့် ပြားပေါ်ကို တစ်သက်တည်း uniform ထားသော force တစ်ခုကို သတ်မှတ်နိုင်သည်။

  - <img alt="" src=images/FEM_ConstraintPressure.svg  style="width:32px;"> [Pressure load](FEM_ConstraintPressure.md): pressure constraint တစ်ခု သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintCentrif.svg  style="width:32px;"> [Centrifugal load](FEM_ConstraintCentrif.md): centrifugal body load constraint ကို သတ်မှတ်ရန် အသုံးပြုသည်။ <small>(v0.20)</small> 

  - <img alt="" src=images/FEM_ConstraintSelfWeight.svg  style="width:32px;"> [Gravity load](FEM_ConstraintSelfWeight.md): ပစ္စည်းပေါ်တွင် လှုပ်ရှားမှုမရှိသော gravity acceleration တစ်ခုကို သတ်မှတ်ရန် အသုံးပြုသည်။

### အပူဂိမ်း ဆိုင်ရာ ကန့်သတ်ချက်များနှင့် လုပ်ဆောင်ချက်များ (Thermal boundary conditions and loads) 

  - <img alt="" src=images/FEM_ConstraintInitialTemperature.svg  style="width:32px;"> [Initial temperature](FEM_ConstraintInitialTemperature.md): ကိုယ်ထည်၏ initial temperature ကို သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintHeatflux.svg  style="width:32px;"> [Heat flux load](FEM_ConstraintHeatflux.md): မျက်နှာ(များ) ပေါ်တွင် heat flux constraint ကို သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintTemperature.svg  style="width:32px;"> [Temperature boundary condition](FEM_ConstraintTemperature.md): point/edge/face(များ) အပေါ် temperature constraint တစ်ခု သတ်မှတ်ရန် အသုံးပြုသည်။

  - <img alt="" src=images/FEM_ConstraintBodyHeatSource.svg  style="width:32px;"> [Body heat source](FEM_ConstraintBodyHeatSource.md): အတွင်းမှ ထွက်ပေါက်လာသော body heat ကို သတ်မှတ်ရန် အသုံးပြုသည်။

### အတိုးပြုပြင်ချင်သော Constants (Overwrite Constants) 

  - <img alt="" src=images/FEM_ConstantVacuumPermittivity.svg  style="width:32px;"> [Constant vacuum permittivity](FEM_ConstantVacuumPermittivity.md): [permittivity of vacuum](https://en.wikipedia.org/wiki/Vacuum_permittivity) ကို ကိုယ့်လိုအပ်သည့် တန်ဖိုးဖြင့် အစားထိုး သတ်မှတ်နိုင်သည်။

  
## Menu: Mesh 

-   <img alt="" src=images/FEM_MeshNetgenFromShape.svg  style="width:32px;"> [FEM mesh from shape by Netgen](FEM_MeshNetgenFromShape.md): Netgen ကို အသုံးပြု၍ မော်ဒယ်အတွက် finite element mesh ကို 생성 (generate) ပြုလုပ်သည်။

-   <img alt="" src=images/FEM_MeshGmshFromShape.svg  style="width:32px;"> [FEM mesh from shape by Gmsh](FEM_MeshGmshFromShape.md): Gmsh ကို အသုံးပြု၍ မော်ဒယ်အတွက် finite element mesh ကို 생성 ပြုလုပ်သည်။

-   <img alt="" src=images/FEM_MeshBoundaryLayer.svg  style="width:32px;"> [FEM mesh boundary layer](FEM_MeshBoundaryLayer.md): ဆန့်ကျင်နယ်နီးများတွင် မှန်ကန်ကျိန်သေမှုများအတွက် anisotropic meshes များ ဖန်တီးသည်။

-   <img alt="" src=images/FEM_MeshRegion.svg  style="width:32px;"> [FEM mesh region](FEM_MeshRegion.md): mesh ထုတ်မည့် ဒေသများကို တိကျစွာ သတ်မှတ်၍ analysis အချိန်ကို ထိရောက်စွာ တိုးတက်စေသည်။

-   <img alt="" src=images/FEM_MeshGroup.svg  style="width:32px;"> [FEM mesh group](FEM_MeshGroup.md): mesh ၏ elements (vertex, edge, surface) များကို group ဖွဲ့၍ label ချထားနိုင်သည်၊ အပြင်ဘက် solvers သို့ export တင်ပို့ရာတွင် 유용 ဖြစ်သည်။

-   <img alt="" src=images/FEM_CreateElementsSet.svg  style="width:32px;"> [Erase Elements](FEM_CreateElementsSet.md): polygon ဖြင့် ရွေးထားသော elements များကို mesh ထဲမှ ဖျက်/ဖျောက်ထားသည်။ <small>(v1.0)</small> 

-   <img alt="" src=images/FEM_FemMesh2Mesh.svg  style="width:32px;"> [FEM mesh to mesh](FEM_FemMesh2Mesh.md): ရွေးချယ်ထားသော FEM mesh ၏ 3D elements များ၏ surface များ သို့မဟုတ် 2D elements အားလုံးကို surface mesh သို့ ပြောင်းလဲပေးသည်။

## Menu: Solve 

-   <img alt="" src=images/FEM_SolverCalculixCxxtools.svg  style="width:32px;"> [Solver CalculiX Standard](FEM_SolverCalculixCxxtools.md): ဤ analysis အတွက် solver controller အသစ်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md): Elmer အတွက် solver controller ကို ဖန်တီးသည်။

-   <img alt="" src=images/FEM_SolverMystran.svg  style="width:32px;"> [Solver Mystran](FEM_SolverMystran.md): MYSTRAN solver အတွက် solver controller ဖန်တီးသည်။ <small>(v0.20)</small> 

-   <img alt="" src=images/FEM_SolverZ88.svg  style="width:32px;"> [Solver Z88](FEM_SolverZ88.md): Z88 အတွက် solver controller ကို ဖန်တီးသည်။

### مکانیک သင်္ချာရင်းများ (Mechanical equations) 

  - <img alt="" src=images/FEM_EquationElasticity.svg  style="width:32px;"> [Elasticity equation](FEM_EquationElasticity.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ linear mechanical analyses များ ဆောင်ရွက်ရန် သင်္ချာရင်းဖြစ်သည်။

  - <img alt="" src=images/FEM_EquationDeformation.svg  style="width:32px;"> [Deformation equation](FEM_EquationDeformation.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) အတွက် nonlinear mechanical analyses (deformations) များ ဆောင်ရွက်ရန် သင်္ချာရင်းဖြစ်သည်။ <small>(v0.21)</small> 

### အလျှပ်စစ် သင်္ချာရင်းများ (Electromagnetic equations) 

  - <img alt="" src=images/FEM_EquationElectrostatic.svg  style="width:32px;"> [Electrostatic equation](FEM_EquationElectrostatic.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ electrostatic analyses များ ဆောင်ရွက်ရန် သင်္ချာရင်းဖြစ်သည်။

  - <img alt="" src=images/FEM_EquationElectricforce.svg  style="width:32px;"> [Electricforce equation](FEM_EquationElectricforce.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ မျက်နှာပေါ်ရှိ electric force ကို တွက်ချက်ရန် သုံးသည်။

  - <img alt="" src=images/FEM_EquationMagnetodynamic.svg  style="width:32px;"> [Magnetodynamic equation](FEM_EquationMagnetodynamic.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ magnetodynamics ကို တွက်ချက်ရန် အသုံးပြုသည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/FEM_EquationMagnetodynamic2D.svg  style="width:32px;"> [Magnetodynamic 2D equation](FEM_EquationMagnetodynamic2D.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ 2D အတွက် magnetodynamics ကို တွက်ချက်ရန် အသုံးပြုသည်။ <small>(v0.21)</small> 

-   <img alt="" src=images/FEM_EquationFlow.svg  style="width:32px;"> [Flow equation](FEM_EquationFlow.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ flow analyses များ ဆောင်ရွက်ရန် သင့်ဖြစ်သည်။

-   <img alt="" src=images/FEM_EquationFlux.svg  style="width:32px;"> [Flux equation](FEM_EquationFlux.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ flux analyses များ ဆောင်ရွက်ရန် သင်္ချာရင်းဖြစ်သည်။

-   <img alt="" src=images/FEM_EquationHeat.svg  style="width:32px;"> [Heat equation](FEM_EquationHeat.md): <img alt="" src=images/FEM_SolverElmer.svg  style="width:32px;"> [Solver Elmer](FEM_SolverElmer.md) ကို အသုံးပြု၍ heat transfer analyses များ ဆောင်ရွက်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_SolverControl.svg  style="width:32px;"> [Solver job control](FEM_SolverControl.md): ရွေးချယ်ထားသော solver ကို စတင်ပြေးစေခြင်းနှင့် ချိန်ညှိရန် မီနူးကို ဖွင့်သည်။

-   <img alt="" src=images/FEM_SolverRun.svg  style="width:32px;"> [Run solver calculations](FEM_SolverRun.md): active analysis ၏ ရွေးချယ်ထားသော solver ကို ပြေးစေသည်။

## Menu: Results 

-   <img alt="" src=images/FEM_ResultsPurge.svg  style="width:32px;"> [Purge results](FEM_ResultsPurge.md): active analysis ၏ ရလဒ်များကို ဖျက်ချသည်။

-   <img alt="" src=images/FEM_ResultShow.svg  style="width:24px;"> [Show result](FEM_ResultShow.md): analysis ရလဒ်ကို ပြသရန် အသုံးပြုသည်။ ဤ dialog ကို [Solver Elmer](FEM_SolverElmer.md) အတွက် မရနိုင်ပါ၊ အဆိုပါ solver သည် [Post pipeline from result](FEM_PostPipelineFromResult.md) object ကိုသာ အသုံးပြုကာ ရလဒ်ကို ဗျူဟာပြသသည်။

-   <img alt="" src=images/FEM_PostApplyChanges.svg  style="width:32px;"> [Apply changes to pipeline](FEM_PostApplyChanges.md): pipelines နှင့် filters များတွင် ပြောင်းလဲမှုများကို ချက်ချင်း အကောင်အထည်ဖော်မည်ဆိုပါက toggle ပြုလုပ်ပေးသည်။

-   <img alt="" src=images/FEM_PostPipelineFromResult.svg  style="width:32px;"> [Post pipeline from result](FEM_PostPipelineFromResult.md): FEM analysis ရလဒ်များအတွက် နောက်ထပ် ဂရပ်ဖစ် ကိုယ်စားပြုမှု (color scale နှင့် ပြသမှု ရွေးချယ်စရာများ) များကို ထည့်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_PostFilterWarp.svg  style="width:32px;"> [Warp filter](FEM_PostFilterWarp.md): မော်ဒယ်၏ ပမာဏကို အရွယ်စားတိုးပြီး ပြောင်းလဲသည့် akshape ကို အမြင်ဖော်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_PostFilterClipScalar.svg  style="width:32px;"> [Scalar clip filter](FEM_PostFilterClipScalar.md): သတ်မှတ်ထားသော scalar တန်ဖိုးဖြင့် field ကို clip ပြုလုပ်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_PostFilterCutFunction.svg  style="width:32px;"> [Function cut filter](FEM_PostFilterCutFunction.md): မော်ဒယ်ကို ဖြတ်ထွက်သော sphere သို့မဟုတ် plane ပေါ်တွင် ရလဒ်ကို ပြသရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_PostFilterClipRegion.svg  style="width:32px;"> [Region clip filter](FEM_PostFilterClipRegion.md): sphere သို့ plane ဖြင့် ဖြတ်ထားသည့် ဒေသတစ်ခုဖြင့် field ကို clip ပြုလုပ်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_PostFilterContours.svg  style="width:32px;"> [Contours filter](FEM_PostFilterContours.md): iso-lines (2D အတွက်) သို့မဟုတ် iso-contours များကို ပြသရန် အသုံးပြုသည်။ <small>(v0.21)</small> 

-   <img alt="" src=images/FEM_PostFilterDataAlongLine.svg  style="width:32px;"> [Line clip filter](FEM_PostFilterDataAlongLine.md): သတ်မှတ်ထားသော line တစ်ခုအလျား field ၏ တန်ဖိုးများကို plot ဆွဲရန် အသုံးပြုသည်။

-   <img alt="" src=images/FEM_PostFilterLinearizedStresses.svg  style="width:32px;"> [Stress linearization plot](FEM_PostFilterLinearizedStresses.md): stress linearization plot ကို ဖန်တီးပေးသည်။

-   <img alt="" src=images/FEM_PostFilterDataAtPoint.svg  style="width:32px;"> [Data at point clip filter](FEM_PostFilterDataAtPoint.md): သတ်မှတ်ထားသော point တစ်ခုတွင် ရှိသော field တန်ဖိုးကို ပြသရန် အသုံးပြုသည်။

### Filter functions 

  - <img alt="" src=images/FEM_PostCreateFunctionPlane.svg  style="width:32px;"> [Plane](FEM_PostCreateFunctionPlane.md): result mesh ကို plane ဖြင့် ဖြတ်လိုက်သည်။

  - <img alt="" src=images/FEM_PostCreateFunctionSphere.svg  style="width:32px;"> [Sphere](FEM_PostCreateFunctionSphere.md): result mesh ကို sphere ဖြင့် ဖြတ်လိုက်သည်။

  - <img alt="" src=images/FEM_PostCreateFunctionCylinder.svg  style="width:32px;"> [Cylinder](FEM_PostCreateFunctionCylinder.md): result mesh ကို cylinder ဖြင့် ဖြတ်လိုက်သည်။ <small>(v0.21)</small> 

  - <img alt="" src=images/FEM_PostCreateFunctionBox.svg  style="width:32px;"> [Box](FEM_PostCreateFunctionBox.md): result mesh ကို box ဖြင့် ဖြတ်လိုက်သည်။ <small>(v0.21)</small> 

## Menu: Utilities 

-   <img alt="" src=images/FEM_ClippingPlaneAdd.svg  style="width:32px;"> [Clipping plane on face](FEM_ClippingPlaneAdd.md): မော်ဒယ် တစ်ခုလုံး၏ ပြသမှုအတွက် clipping plane တစ်ခု ထည့်သွင်းပေးသည်။

-   <img alt="" src=images/FEM_ClippingPlaneRemoveAll.svg  style="width:32px;"> [Remove all clipping planes](FEM_ClippingPlaneRemoveAll.md): ရှိပြီးသား clipping planes ( [Clipping plane on face](FEM_ClippingPlaneAdd.md) ) အားလုံးကို ဖယ်ရှားပေးသည်။

-   <img alt="" src=images/FEM_Examples.svg  style="width:32px;"> [Open FEM examples](FEM_Examples.md): FEM examples များကို ဝင်ရောက်ကြည့်ရှုရန် GUI ကို ဖွင့်ပေးသည်။

## Context Menu 

-   <img alt="" src=images/FEM_MeshClear.svg  style="width:32px;"> [Clear FEM mesh](FEM_MeshClear.md): FreeCAD ဖိုင်မှ mesh ဖိုင်ကို ဖျက်မည်။ FreeCAD ဖိုင်ကို ပိုလှပေအောင် ထိန်းချုပ်ရန် အသုံးဝင်သည်။

-   <img alt="" src=images/FEM_MeshDisplayInfo.svg  style="width:32px;"> [Display FEM mesh info](FEM_MeshDisplayInfo.md): ရှိပြီးသား mesh ၏ မူလစာရင်းအချက်အလက် များကို ပြသသည် - nodes အရေအတွက်နှင့် element အမျိုးအစားအလိုက် အရေအတွက်များ။

## မရေရာသေးသော ကိရိယာများ (Obsolete tools) 

-   <img alt="" src=images/FEM_ConstraintFluidBoundary.svg  style="width:32px;"> [Fluid boundary condition](FEM_ConstraintFluidBoundary.md): fluid boundary condition ကို သတ်မှတ်ရန် အသုံးပြုသည်။ solver မရှိသေးသည်။ <small>(v1.0)</small> တွင် မရရှိနိုင်တော့။

-   <img alt="" src=images/FEM_ConstraintBearing.svg  style="width:32px;"> [Constraint bearing](FEM_ConstraintBearing.md): bearing constraint ကို သတ်မှတ်ရန် အသုံးပြုသည်။ solver မရှိသေး၍ မရရှိနိုင်ခဲ့သည်။ <small>(v1.0)</small> တွင် မရရှိနိုင်တော့။

-   <img alt="" src=images/FEM_ConstraintGear.svg  style="width:32px;"> [Constraint gear](FEM_ConstraintGear.md): gear constraint ကို သတ်မှတ်ရန် အသုံးပြုသည်။ solver မရှိသေး၍ မရရှိနိုင်ခဲ့သည်။ <small>(v1.0)</small> တွင် မရရှိနိုင်တော့။

-   <img alt="" src=images/FEM_ConstraintPulley.svg  style="width:32px;"> [Constraint pulley](FEM_ConstraintPulley.md): pulley constraint ကို သတ်မှတ်ရန် အသုံးပြုသည်။ solver မရှိသေး၍ မရရှိနိုင်ခဲ့သည်။ <small>(v1.0)</small> တွင် မရရှိနိုင်တော့။

-   <img alt="" src=images/FEM_SolverCalculiX.svg  style="width:32px;"> [Solver CalculiX (new framework)](FEM_SolverCalculiX.md): မူလ framework ဖြစ်သော <img alt="" src=images/FEM_SolverCalculixCxxtools.svg  style="width:32px;"> [Solver CalculiX Standard](FEM_SolverCalculixCxxtools.md) နှင့် တူညီသော်လည်း အပိုစစ်ဆေးချက်များပါရှိသည်။ ကိရိယာသည် ပြီးစီးမှု မရခဲ့သဖြင့် <small>(v1.0)</small> တွင် မရရှိနိုင်ထားပါ။

-   <img alt="" src=images/FEM_CreateNodesSet.svg  style="width:32px;"> [Nodes set](FEM_CreateNodesSet.md): FEM mesh မှ node set တစ်ခု ဖန်တီး/သတ်မှတ်ပေးသည်။ ကိရိယာသည် ပြီးစီးမှု မရှိ၍ အသုံးမပြုနိုင်ခဲ့သည်။ <small>(v1.0)</small> တွင် မရရှိနိုင်ပါ။

## Preferences

-   <img alt="" src=images/Std_DlgPreferences.svg  style="width:32px;"> [Preferences\...](FEM_Preferences.md): FEM Tools တွင် ရရှိနိုင်သည့် preferences များ။

## အချက်အလက်

အောက်ပါ စာမျက်နှာများသည် FEM Workbench ၏ မတူကွဲပြားသည့် ခေါင်းစဉ်များကို ရှင်းပြသည်။

[FEM Install](FEM_Install.md): workbench တွင် အသုံးပြုသည့် အပြင်ဘက် အစီအစဉ်များကို သတ်မှတ်ရန် အသေးစိတ် ဖော်ပြချက်။

[FEM Geometry Preparation and Meshing](FEM_Geometry_Preparation_and_Meshing.md): FEM နှင့် meshing အတွက် geometry ပြင်ဆင်ခြင်းဆိုင်ရာ အကြံပေးချက်များ။

[FEM Mesh](FEM_Mesh.md): FEM workbench တွင် mesh များအကြောင်း အသေးစိတ်။

[FEM Solver](FEM_Solver.md): workbench တွင် ရရှိနိုင်သည့် solvers များနှင့် အနာဂတ်တွင် အသုံးပြုနိုင်သည့် solvers များအကြောင်း ပိုမိုသိရှိရန်။

[FEM CalculiX](FEM_CalculiX.md): structural analysis အတွက် workbench တွင် ပုံမှန်အသုံးပြုသော CalculiX အကြောင်း ပိုမိုသိရှိရန်။

[FEM Concrete](FEM_Concrete.md): ကြမ်းတမ်းသော အဆောက်အအုံများကို စမ်းသပ်မှုဆိုင်ရာ စိတ်ဝင်စားဖွယ် အချက်အလက်များ။

## သင်တန်းများ (Tutorials)

Tutorial 1: [FEM CalculiX Cantilever 3D](FEM_CalculiX_Cantilever_3D.md); အခြေချထားထားသော schlicht supported beam analysis ထိန်းချုပ်မှု။

Tutorial 2: [FEM Tutorial](FEM_tutorial.md); တည်ဆောက်မှုတစ်ခု၏ ရိုးရှင်းသည့် တင်းရှည်ခြင်း (tension) စစ်ဆေးမှု။

Tutorial 3: [FEM Tutorial Python](FEM_Tutorial_Python.md); cantilever ဥပမာကို အပြည့်အစုံ Python scripting ဖြင့် စတင် တည်ဆောက်ခြင်း၊ mesh အပါအဝင်။

Tutorial 4: [FEM Shear of a Composite Block](FEM_Shear_of_a_Composite_Block.md); နှစ်မျိုးသော ပစ္စည်းများ ဖွဲ့စည်းထားသည့် block ၏ deformation ကို ကြည့်ရှုရန်။

Tutorial 5: [Transient FEM analysis](Transient_FEM_analysis.md)

Tutorial 6: [Post-Processing of FEM Results with Paraview](Post-Processing_of_FEM_Results_with_Paraview.md)

Tutorial 7: [FEM Example Capacitance Two Balls](FEM_Example_Capacitance_Two_Balls.md); Elmer ၏ GUI tutorial 6 "Electrostatics Capacitance Two Balls" ကို FEM Examples မှ အသုံးပြု၍ ဖော်ပြထားသည်။

Coupled thermal mechanical analysis tutorials by [openSIM](https://opensimsa.github.io/training.html)

Video tutorial 1: [FEM video for beginner](https://forum.freecadweb.org/viewtopic.php?f=18&t=20499#p158353) (YouTube link ပါဝင်သည်)

Video tutorial 2: [FEM video for beginner](https://forum.freecadweb.org/viewtopic.php?f=18&t=20499&start=10#p162321) (YouTube link ပါဝင်သည်)

Many video tutorials: [anisim Open Source Engineering Software](https://www.youtube.com/channel/UCnvFCm2BbXOVI3ObfXcxXhw) (ဂျာမန်ဘာသာဖြင့်)

## FEM Workbench ကို ထပ်ချဲ့ခြင်း (Extending the FEM Workbench) 

FEM Workbench ကို အချိန်တိုင်း တိုးတက်အဆင့်မြှင့် လုပ်ဆောင်နေသည်။ ပရောဂျက်၏ ရည်မှန်းချက်တစ်ခုမှာ မျိုးစုံသော FEM solvers များနှင့် လွယ်ကူစွာ အပြန်အလှန် အလုပ်လုပ်နိုင်စေရန်နည်းလမ်းများရှာဖွေခြင်းဖြစ်သည်၊ ထို့ကြောင့် အသုံးပြုသူသည် ဖရီးကက် (FreeCAD) အတွင်းတွင် အစပြု၊ meshing၊ simulation နှင့် optimization ဆောင်ရွက်မှုများကို တစ်နှစ်လုံး ပိုမို စနစ်တကျ ပြုလုပ်နိုင်သည်။

အောက်ပါ အချက်အလက်များသည် FEM Workbench ကို မတူကွဲပြားစွာ တိုးချဲ့လိုသူ power users နှင့် developer များအတွက် ဖြစ်သည်။ C++ နှင့် Python အသာကြီးများကို သိရှိမှု၊ နှင့် FreeCAD ၌ အသုံးပြုသော "document object" စနစ်အကြောင်း အနည်းငယ် သိရှိထားမှု လိုအပ်ပါသည်; ဤအချက်အလက်များသည် [Power users hub](Power_users_hub.md) နှင့် [Developer hub](Developer_hub.md) တွင် ရနိုင်သည်။ FreeCAD သည် လက်ရှိ တိုးတက်ဖွံ့ဖြိုးဆဲဖြစ်သဖြင့် အဆိုပါ ဆောင်းပါးအချို့သည် ဟောင်းပြီး အသုံးမပြုနိုင်သဖြစ်နိုသည်။ အထူးသတ်မှတ်ချက်များနှင့် နောက်ဆုံး အချက်အလက်များကို [FreeCAD forums](https://forum.freecadweb.org/index.php) ၏ Development အပိုင်းတွင် ဆွေးနွေးထားသည်။ FEM အကြောင်း ဆွေးနွေးချင်သူများအနေဖြင့် [FEM subforum](https://forum.freecadweb.org/viewforum.php?f=18) ကို ရောက်လေ့လာပါ။

workbench ကို ဘယ်လို တိုးချဲ့နိုင်သည်ဆိုသည်ကို ရှင်းပြသည့် ဆောင်းပါးများမှာ ဥပမာအားဖြင့် ရ boundary conditions (constraints) အသစ်များ ထည့်သွင်းခြင်း သို့မဟုတ် equations အသစ်များ ထည့်သွင်းခြင်းကဲ့သို့ အရာများကို လေ့လာရန် အကူအညီ ဖြစ်သည်။

-   [Extend FEM Module](Extend_FEM_Module.md)
-   [Onboarding FEM Devs](Onboarding_FEM_Devs.md) သည် FEM workbench သို့ အဆင်ပြေစွာ ထည့်သွင်းလိုသူ developer အသစ်များကို လမ်းညွှန်ပေးရန် ရည်ရွယ်သည်။
-   [Add FEM Constraint Tutorial](Add_FEM_Constraint_Tutorial.md)
-   [Add FEM Equation Tutorial](Add_FEM_Equation_Tutorial.md)

Power users များကို FreeCAD ၏ ကုဒ်အခြေခံနှင့် core elements များနှင့် workbenches တို့အကြား လှုပ်ရှားမှုများကို နားလည်စေ ပေးရန် developer ဂိုဏ်းလမ်းညွှန်စာအုပ်တစ်အုပ်ရေးသားထားသည်။ ဤစာအုပ်ကို GitHub တွင် ဧည့်ခံထားပြီး အများအသုံးပြုသူများ တက်ကြွစွာ ဖြည့်စွက် ပြင်ဆင်နိုင်သည်။

-   [Early preview of ebook: Module developer\' guide to FreeCAD source](https://forum.freecadweb.org/viewtopic.php?t=17581) forum thread.
-   [FreeCAD Mod Dev Guide](https://github.com/qingfengxia/FreeCAD_Mod_Dev_Guide) github repository.

## FEM Workbench စာတမ်းများကို ထပ်ချဲ့ရေးသားခြင်း (Extending the FEM Workbench documentation) 

-   FEM documentation ထဲတွင် ထပ်ရေးသင့်သော်လည်း မရှိသေးသော အချက်အလက်များကို forum တွင် ရှာတွေ့နိုင်သည်: [FEM documentation missing on the Wiki](https://forum.freecadweb.org/viewtopic.php?f=18&t=20823)




 {{FEM Tools navi}}



---
⏵ [documentation index](../README.md) > [Workbenches](Category_Workbenches.md) > [FEM](Category_FEM.md) > FEM Workbench