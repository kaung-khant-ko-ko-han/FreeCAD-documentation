**ရိုဘော့ လုပ်ငန်းခွင် (Robot Workbench) ကို လက်ရှိတွင် ထိန်းသိမ်းစောင့်ရှောက်သူ (maintainer) မရှိပါ။ အကယ်၍ သင်သည် ဤဘာသာရပ်နှင့် ပတ်သက်၍ အတွေ့အကြုံရှိပြီး ၎င်းကို ထိန်းသိမ်းရန် စိတ်ဝင်စားပါက၊ [ဖရီးကက် ဖိုရမ် (FreeCAD forum)](https://forum.freecadweb.org/index.php) ၏ developer ကဏ္ဍတွင် သင်၏ ဆန္ဒကို အသိပေးနိုင်ပါသည်။**

**ဤလုပ်ငန်းခွင်ကို ပင်မရင်းမြစ်ကုဒ် (master source code) တွင် ဆက်လက်ထားရှိရခြင်း အကြောင်းရင်းမှာ ၎င်းကို C++ ဖြင့် ရေးသားထားသောကြောင့် ဖြစ်ပါသည်။ အကယ်၍ ဤလုပ်ငန်းခွင်ကို ပိုင်သွန် (Python) ဖြင့် ရေးသားနိုင်ပါက၊ ၎င်းကို [ပြင်ပ လုပ်ငန်းခွင် (external workbench)](external_workbenches.md) အဖြစ် ပြုလုပ်နိုင်ပြီး သီးခြား repository တစ်ခုသို့ ရွှေ့ပြောင်းနိုင်မည် ဖြစ်ပါသည်။**

## နိဒါန်း (Introduction)

 <img alt=" Robot workbench icon" src=images/Workbench_Robot.svg  style="width:128px;"> 

<img alt="" src=images/Workbench_Robot.svg  style="width:24px;"> [ရိုဘော့ လုပ်ငန်းခွင် (Robot Workbench)](Robot_Workbench.md) သည် [Kuka](http://kuka.com/) ကဲ့သို့သော စံနှုန်းမီ [၆-ဝင်ရိုးသုံး စက်မှုရိုဘော့ (6-axis industrial robot)](Robot_6-Axis.md) တစ်ခုကို ပုံဖော်စမ်းသပ်ရန် (simulate) အသုံးပြုသော ကိရိယာတစ်ခု ဖြစ်ပါသည်။

သင်သည် အောက်ပါလုပ်ငန်းများကို ဆောင်ရွက်နိုင်ပါသည် -

-   ရိုဘော့နှင့် အလုပ်လုပ်မည့် အစိတ်အပိုင်းများ (work pieces) ပါဝင်သော ပုံဖော်စမ်းသပ်မှု ပတ်ဝန်းကျင်တစ်ခုကို တည်ဆောက်ခြင်း။
-   ရွေ့လျားမှု လမ်းကြောင်းများ (movement trajectories) ကို ဖန်တီးခြင်းနှင့် ဖြည့်သွင်းခြင်း။
-   CAD အစိတ်အပိုင်းတစ်ခု၏ အင်္ဂါရပ်များကို လမ်းကြောင်းတစ်ခုအဖြစ် ခွဲထုတ်ခြင်း။
-   ရိုဘော့၏ ရွေ့လျားမှုနှင့် လက်လှမ်းမီနိုင်သော အကွာအဝေးကို ပုံဖော်စမ်းသပ်ခြင်း။
-   လမ်းကြောင်းကို ရိုဘော့ပရိုဂရမ်ဖိုင်အဖြစ် တင်ပို့ခြင်း (export)။

စတင်အသုံးပြုရန် [ရိုဘော့ လေ့ကျင့်ခန်းလမ်းညွှန် (Robot tutorial)](Robot_tutorial.md) ကို စမ်းသပ်ကြည့်ပါ၊ နှင့် [RobotExample.py](https://github.com/FreeCAD/FreeCAD_sf_master/blob/master/src/Mod/Robot/RobotExample.py) နမူနာဖိုင်ရှိ programming interface ကို ကြည့်ရှုနိုင်ပါသည်။

## ကိရိယာများ (Tools)

ရိုဘော့ တည်ဆောက်မှုတစ်ခု ဖန်တီးရန် သင်အသုံးပြုနိုင်သော အဓိက အမိန့်ပေးချက်များမှာ အောက်ပါအတိုင်း ဖြစ်ပါသည်။

### ရိုဘော့များ (Robots)

၆-ဝင်ရိုးသုံး ရိုဘော့များကို ဖန်တီးရန်နှင့် စီမံခန့်ခွဲရန် ကိရိယာများ -

-   <img alt="" src=images/Robot_CreateRobot.svg  style="width:30px;"> [ရိုဘော့တစ်ခု ဖန်တီးခြင်း (Create a robot)](Robot_CreateRobot.md): မြင်ကွင်းထဲသို့ ရိုဘော့အသစ်တစ်ခု ထည့်သွင်းခြင်း။
-   <img alt="" src=images/Robot_Simulate.svg  style="width:30px;"> [လမ်းကြောင်းတစ်ခုကို ပုံဖော်စမ်းသပ်ခြင်း (Simulate a trajectory)](Robot_Simulate.md): ပုံဖော်စမ်းသပ်မှု ဒိုင်ယာလော့ဂ်ကို ဖွင့်ပြီး စမ်းသပ်မှုများ ပြုလုပ်ခြင်း။
-   <img alt="" src=images/Robot_Export.svg  style="width:30px;"> [လမ်းကြောင်းတစ်ခုကို တင်ပို့ခြင်း (Export a trajectory)](Robot_Export.md): ရိုဘော့ပရိုဂရမ်ဖိုင်တစ်ခု တင်ပို့ခြင်း။
-   <img alt="" src=images/Robot_SetHomePos.svg  style="width:30px;"> [မူလနေရာ သတ်မှတ်ခြင်း (Set home position)](Robot_SetHomePos.md): ရိုဘော့၏ မူလနေရာ (home position) ကို သတ်မှတ်ခြင်း။
-   <img alt="" src=images/Robot_RestoreHomePos.svg  style="width:30px;"> [မူလနေရာသို့ ပြန်သွားခြင်း (Restore home position)](Robot_RestoreHomePos.md): ရိုဘော့ကို ၎င်း၏ မူလနေရာသို့ ရွှေ့ပြောင်းခြင်း။

### လမ်းကြောင်းများ (Trajectories)

လမ်းကြောင်းများကို ဖန်တီးရန်နှင့် ကိုင်တွယ်ရန် ကိရိယာများ။ ပါရာမက်ထရစ် (parametric) နှင့် ပါရာမက်ထရစ် မဟုတ်သော (non parametric) ဟူ၍ နှစ်မျိုးရှိပါသည်။

#### ပါရာမက်ထရစ် မဟုတ်သော လမ်းကြောင်းများ (Non parametric trajectories)

-   <img alt="" src=images/Robot_CreateTrajectory.svg  style="width:30px;"> [လမ်းကြောင်းတစ်ခု ဖန်တီးခြင်း (Create a trajectory)](Robot_CreateTrajectory.md): မြင်ကွင်းထဲသို့ အလွတ်ဖြစ်သော လမ်းကြောင်းအရာဝတ္ထုအသစ်တစ်ခု ထည့်သွင်းခြင်း။
-   <img alt="" src=images/Robot_SetDefaultOrientation.svg  style="width:30px;"> [စံနှုန်းအတိုင်း တည်ရှိပုံကို သတ်မှတ်ခြင်း (Set the default orientation)](Robot_SetDefaultOrientation.md): way-points များ စတင်ဖန်တီးချိန်တွင် ရှိနေရမည့် တည်ရှိပုံကို သတ်မှတ်ခြင်း။
-   <img alt="" src=images/Robot_SetDefaultValues.svg  style="width:30px;"> [စံနှုန်းအတိုင်း အမြန်နှုန်း ကန့်သတ်ချက်ကို သတ်မှတ်ခြင်း (Set the default speed parameter)](Robot_SetDefaultValues.md): way-point ဖန်တီးမှုအတွက် စံနှုန်းတန်ဖိုးများကို သတ်မှတ်ခြင်း။
-   <img alt="" src=images/Robot_InsertWaypoint.svg  style="width:30px;"> [လမ်းကြောင်းအမှတ်တစ်ခု ထည့်သွင်းခြင်း (Insert a waypoint)](Robot_InsertWaypoint.md): လက်ရှိ ရိုဘော့တည်နေရာမှ လမ်းကြောင်းအမှတ် (way-point) တစ်ခုကို လမ်းကြောင်းထဲသို့ ထည့်သွင်းခြင်း။
-   <img alt="" src=images/Robot_InsertWaypointPre.svg  style="width:30px;"> [ရွေးချယ်ထားသော လမ်းကြောင်းအမှတ်ကို ထည့်သွင်းခြင်း (Insert a waypoint preselected)](Robot_InsertWaypointPre.md): လက်ရှိ မောက်စ်တည်နေရာမှ လမ်းကြောင်းအမှတ်တစ်ခုကို လမ်းကြောင်းထဲသို့ ထည့်သွင်းခြင်း။

#### ပါရာမက်ထရစ် လမ်းကြောင်းများ (Parametric trajectories)

-   <img alt="" src=images/Robot_Edge2Trac.svg  style="width:30px;"> [အနားသတ်များမှ လမ်းကြောင်းတစ်ခု ဖန်တီးခြင်း (Create a trajectory out of edges)](Robot_Edge2Trac.md): အနားသတ်များကို လမ်းကြောင်းတစ်ခုအဖြစ် ခွဲထုတ်ပေးသော အရာဝတ္ထုအသစ်တစ်ခု ထည့်သွင်းခြင်း။
-   <img alt="" src=images/Robot_TrajectoryDressUp.svg  style="width:30px;"> [လမ်းကြောင်းကို အလှဆင်ခြင်း (Dress-up a trajectory)](Robot_TrajectoryDressUp.md): လမ်းကြောင်းတစ်ခု၏ ဂုဏ်သတ္တိ တစ်ခု သို့မဟုတ် တစ်ခုထက်ပိုသည်ကို ပြောင်းလဲသတ်မှတ်ခွင့်ပေးခြင်း။
-   <img alt="" src=images/Robot_TrajectoryCompound.svg  style="width:30px;"> [လမ်းကြောင်းအစုအဝေး (Trajectory compound)](Robot_TrajectoryCompound.md): တစ်ခုချင်းစီဖြစ်သော လမ်းကြောင်းအချို့မှ အစုအဝေးတစ်ခု ဖန်တီးခြင်း။

## စခရစ်ရေးသားခြင်း (Scripting)

ရိုဘော့၏ ရွှေ့လျားမှုများကို ပုံဖော်ရန် အသုံးပြုသော လုပ်ဆောင်ချက်များ၏ ရှင်းလင်းချက်အတွက် [ရိုဘော့ API နမူနာ (Robot API example)](Robot_API_example.md) ကို ကြည့်ရှုပါ။

## လေ့ကျင့်ခန်းလမ်းညွှန်များ (Tutorials)

-   [၆-ဝင်ရိုးသုံး ရိုဘော့ (Robot 6-Axis)](Robot_6-Axis.md)
-   [ရိုဘော့ ပုံဖော်စမ်းသပ်မှုအတွက် VRML ပြင်ဆင်ခြင်း (VRML Preparation for Robot Simulation)](VRML_Preparation_for_Robot_Simulation.md)

---
⏵ [မှတ်တမ်း အညွှန်း (documentation index)](../README.md) > [လုပ်ငန်းခွင်များ (Workbenches)](Category_Workbenches.md) > [ရိုဘော့ (Robot)](Category_Robot.md) > ရိုဘော့ လုပ်ငန်းခွင် (Robot Workbench)
