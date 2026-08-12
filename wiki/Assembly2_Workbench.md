# Assembly2 လုပ်ငန်းခွင် (Workbench)
**Assembly2 လုပ်ငန်းခွင်သည် အသစ်မဟုတ်တော့ပါ။ ၎င်းကို ရေးသားသူက အားမထုတ်ပြန်ဖြန့်ဖြူးတော့သဖြင့် FreeCAD ဗားရှင်း 0.17 နှင့်အထက်များတွင် အလုပ်မလုပ်နိုင်နိုင်ပါသဖြင့် ကန့်သတ်ချက်ရှိနိုင်ပါသည်။ ဤ စာမျက်နှာအပါအဝင် သတင်းအချက်အလက်များကို ပြန်လည် ပြင်ဆင်မထားပါ; သမိုင်းဆိုင်ရာ ရည်ရွယ်ချက်အတွက်သာ သိမ်းဆည်းထားသည်။**


{{Message|အစားထိုးရွေးချယ်စရာအဖြစ် [A2plus](A2plus_Workbench.md) ကို ကြည့်ပါ။ ထိုလုပ်ငန်းခွင်သည် Assembly2 ၏ fork ဖြစ်သော်လည်း အပြန်အလှန်ကိုက်ညီမှု မရှိပါ။ ရှေးအမျိုးအစား မော်ဒယ်များကို ဖွင့်ရန်လိုအပ်ပါက FreeCAD 0.16 နှင့် Assembly2 ကို အသုံးပြုနေထိုင်သင့်သည်။ နောက်ဆက်တွဲ မော်ဒယ်အသစ်များကို အစအဆုံး A2plus ဖြင့် ဖန်တီး၍ ဖွင့်သင့်ပါသည်။<br/>


အခြား ရွေးချယ်စရာများအတွက် [Assembly3](Assembly3_Workbench.md) သို့မဟုတ် [Assembly4](Assembly4_Workbench.md) ကို ကြည့်ပါ။ ဤလုပ်ငန်းခွင်များလည်း Assembly2 မှ အားပေးသံပုဒ်ရထားသော်လည်း Assembly2 နှင့် ကိုက်ညီမှု မရှိပါ။}}

## နိဒါန်း

[Assembly2](Assembly2_Workbench.md) သည် ဖရီးကက် (FreeCAD) v0.15 အတွက် အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly) လုပ်ငန်းခွင် (Workbench) ဖြစ်ပြီး ပြင်ပ ဖိုင်များမှ အစိတ်အပိုင်းများကို ထည့်သွင်းနိုင်စေသည်။

၎င်း၏ရေးသားသူက [ဖိုရမ်တွင်](https://forum.freecadweb.org/viewtopic.php?f=17&t=16591) ပြောကြားထားသလို 2016 ခုနှစ်မှစ၍ ထိန်းသိမ်းမထားတော့ပါ၊ ထို့ကြောင့် FreeCAD 0.17 နှင့်အထက်တွင်ပြဿနာများရှိနိုင်ပါသည်။ ယင်းအစား အသစ်နှင့် လက်ရှိထိန်းသိမ်းနေသော [A2plus လုပ်ငန်းခွင် (Workbench)](A2plus_Workbench.md) သည် ကောင်းမွန်သော အစားထိုးဖြစ်သည်။

![](images/Assembly2_example.jpg )

## အသုံးပြုမှု

ရည်ရွယ်ထားသော အလုပ်စဉ် (Intended work-flow):

- အစိတ်အပိုင်းတိုင်းကို သူ့ကိုယ်ပိုင် ဖရီးကက် (FreeCAD) ဖိုင်အတွင်းတွင် ဒီဇိုင်းရေးဆွဲသည်။
- သီးခြား assembly ဖိုင် (assembly FreeCAD file) တစ်ခု ဖန်တီးထားသည်။
- Assembly 2 လုပ်ငန်းခွင် (Workbench) ကို အသုံးပြုပြီး အစိတ်အပိုင်းများကို ဤ assembly ဖိုင်ထဲသို့ တင်သွင်း (import) လုပ်သည်။
- တင်သွင်းထားသော အစိတ်အပိုင်းများကို ပေါင်းစည်းရန် နေရာဆိုင်ရာ ကန့်သတ်ချက်များ (ကန့်သတ်ချက် (Constraint)) ထည့်သွင်းသည်။

အင်္ဂါရပ်များ (Features)

- circular edge ကန့်သတ်ချက် (circular edge constraint)
- axial ကန့်သတ်ချက် (axial constraint)
- plane ကန့်သတ်ချက် (plane constraint)
- အစိတ်အပိုင်း တင်သွင်းခြင်း (part importing)
- တင်သွင်းပြီးသား အစိတ်အပိုင်းများ အပ်ဒိတ်လုပ်နိုင်ခြင်း

ကန့်သတ်ချက်များ (Limitations)

- ကန့်သတ်ချက်များကို ဖြေရှင်းသည့် solver အရည်အသွေး မကောင်းသဖြင့် စပ်လျဉ်းသော assembly များတွင် မဖြေရှင်းနိုင်လျှင် မလျော့ချ၊ သို့မဟုတ် အလွန်ကြာမြင့်နိုင်သည်။
- undo နှင့် ဆင်တူသော အင်္ဂါရပ်များ မထောက်ပံ့ပါ။

## ကိုးကားချက်များ

- စာရေးသူ: hamish
- မူပိုင်မူ မူလစာမျက်နှာ: [Assembly2](https://github.com/hamish2014/FreeCAD_assembly2)
- GitHub ပေါ်မှ မူကြမ်းကိုး: [Assembly2](https://github.com/hamish2014/FreeCAD_assembly2)

## ကိရိယာများ (Tools)

တူးလ်ဘား / Toolbar

![](images/Assembly2-menu-orizz.png )

အောက်ဆင်း မီနူး (Drop down menu)

![](images/Assembly2-menu-vert.png )

-   <img alt="" src=images/Assembly2_ImportPart.png  style="width:32px;"> ဖရီးကက် (FreeCAD) အခြားစာရွက်မှ အစိတ်အပိုင်း တင်သွင်းရန်
-   <img alt="" src=images/Assembly2_UpdatePart.png  style="width:32px;"> assembly ထဲသို့ တင်သွင်းထားသော အစိတ်အပိုင်းများကို အပ်ဒိတ်လုပ်ရန်
-   <img alt="" src=images/Assembly2_Move.png  style="width:32px;"> ရွှေ့ရန် (Move)
-   <img alt="" src=images/Assembly2_CircularEdgeConstraint.png  style="width:32px;"> စက်ဝိုင်း အနား ကန့်သတ်ချက် ထည့်ရန်
-   <img alt="" src=images/Assembly2_PlaneConstraint.png  style="width:32px;"> မျက်နှာပြင် ကန့်သတ်ချက် ထည့်ရန်
-   <img alt="" src=images/Assembly2_AxialConstraint.png  style="width:32px;"> အလျာလိုက် ကန့်သတ်ချက် ထည့်ရန်
-   <img alt="" src=images/Assembly2_AngularConstraint.png  style="width:32px;"> မျက်နှာပြင်နှစ်ခုအကြား ထောင့်ဆိုင်ရာ ကန့်သတ်ချက် ဖန်တီးရန်
-   <img alt="" src=images/Assembly2_SphericalSurfaceConstraint.png  style="width:32px;"> ဘောပုံမျက်နှာပြင် ကန့်သတ်ချက် ထည့်ရန်
-   <img alt="" src=images/Assembly2_DOFAnimation.png  style="width:32px;"> လွတ်လပ်မှုအဆင့်များ (degrees of freedom) ကို အနိမ့်အမြင့် animate လုပ်ရန်
-   <img alt="" src=images/Assembly2_Assembly2Constraint.png  style="width:32px;"> Assembly2 ကန့်သတ်ချက် (Constraint) ကို ဖြေရှင်းရန်
-   <img alt="" src=images/Assembly2_Mux.png  style="width:32px;"> assembly ကို တစ်ခုတည်းသော object အဖြစ် ပေါင်းစပ်ရန် (ဥပမာ assembly ၏ ပုံဆွဲရန် သုံးနိုင်သည်၊ စသည်...)
-   <img alt="" src=images/Assembly2_ListParts.png  style="width:32px;"> assembly2 လုပ်ငန်းခွင် (Workbench) ဖြင့် တင်သွင်းထားသော objects များမှ အစိတ်အပိုင်း စာရင်း ဖန်တီးရန်
-   <img alt="" src=images/Assembly2_Ceck.png  style="width:32px;"> အစိတ်အပိုင်းများ ထပ်ထွက်/တိုက်မှု (overlap/interference) ရှိမရှိ စစ်ဆေးရန်

အခြားများ (Other)

-   <img alt="" src=images/Assembly2_BoltMultipleCircularEdges.png  style="width:32px;"> စက်ဝိုင်း အနားများစွာကို Bolt ချရန်
-   <img alt="" src=images/Assembly2_FlipConstraint.png  style="width:32px;"> ကန့်သတ်ချက် ပြောင်းဖလှယ်ရန် (Flip constraint)
-   <img alt="" src=images/Assembly2_LockRotation.png  style="width:32px;"> လှည့်လှည့်မှုကို ဘတ်ထည် (lock rotation)
-   <img alt="" src=images/Assembly2_Preferences.png  style="width:32px;"> အနှစ်သာရများ (Preferences)
-   <img alt="" src=images/Assembly2_Assembly2.png  style="width:32px;"> Assembly2 လုပ်ငန်းခွင် အိုင်ကွန် (WB icon)

## တပ်ဆင်ခြင်း (Installation)

### အလိုအလျောက် တပ်ဆင်ခြင်း (Automatic installation)

ဤ လုပ်ငန်းခွင်ကို [Addon Manager](Std_AddonMgr.md) မှတဆင့် တပ်ဆင်နိုင်သည်။

### GitHub မှတဆင့် (From GitHub)

ဤ လုပ်ငန်းခွင်ကို အသုံးပြုရန် သင့် ဖရီးကက် (FreeCAD) Mod ဖိုလ်ဒါအောက်တွင် ဤ git repository ကို clone လုပ်၍ pyside နှင့် numpy Python ပက်ကေ့ဂျ်များကို တပ်ဆင်ရန် လိုအပ်ပါသည်။ Ubuntu ကဲ့သို့ Debian အခြေပြု Linux စနစ်တစ်ခုတွင် BASH မှတဆင့် တပ်ဆင်နိုင်သည် - အောက်ပါအတိုင်း


```python
sudo apt-get install git python-numpy python-pyside
mkdir ~/.FreeCAD/Mod
cd ~/.FreeCAD/Mod
git clone https://github.com/hamish2014/FreeCAD_assembly2.git
```

ဖရီးကက် (FreeCAD) တွင် ယခုအခါ \"Assembly 2\" ဟု အမည်ရသော လုပ်ငန်းခွင် ပေါင်းထည့်မှု အသစ်တစ်ခု ကို တွေ့ရမည်။ တပ်ဆင်ပြီးပါက BASH ဖြင့် git ကို အသုံးပြု၍ နောက်ဆုံးဗားရှင်းသို့ အပ်ဒိတ် (upgrade) ပြုလုပ်နိုင်သည် - အောက်ပါအတိုင်း


```python
cd ~/.FreeCAD/Mod/FreeCAD_assembly2
git pull
rm *.pyc
```

အခြားအဖြစ် Ubuntu စနစ်ပေါ်တွင် freecad-community PPA ကို အသုံးပြုနိုင်ပါသည် -


```python
Add ppa:freecad-community/ppa to your software sources
sudo apt-get update
sudo apt-get install freecad-extras-assembly2
```

Windows တွင်

-   git repository ကို ZIP အဖြစ် ဒေါင်းလုဒ် ပြုလုပ်ပါ
-   သင်၏ ဖရီးကက် (FreeCAD) ကို \"C:\\PortableApps\\FreeCAD 0_15\" တွင် တပ်ဆင်ထားသည်ဟု ယူဆပါက၊ Windows Explorer တွင် \"C:\\PortableApps\\FreeCAD 0_15\\Mod\" သို့ သွားပါ
-   \"assembly2\" ဟု အမည်သစ် ဖိုလ်ဒါ တစ်ခု ဖန်တီးပါ
-   ဒေါင်းလုဒ် ပြုလုပ်ထားသော repository ကို \"C:\\PortableApps\\FreeCAD 0_15\\Mod\\assembly2\\\" ထဲသို့ unzip လုပ်ပါ

ဖရီးကက် (FreeCAD) တွင် ယခုအခါ \"Assembly 2\" ဟု အမည်ရသော လုပ်ငန်းခွင် တစ်ခုကို တွေ့ရမည်ဖြစ်သည်။

Pyside နှင့် Numpy သည် FreeCAD 0.15 dev-Snapshots များတွင် ပေါင်းစည်းထည့်သွင်းထားသဖြင့် ထို Python package များကို သီးခြား တပ်ဆင်ရန် မလိုအပ်ပါ။

နောက်ဆုံးဗားရှင်းသို့ အပ်ဒိတ်လုပ်ရန် assembly2 ဖိုလ်ဒါကို ဖျက်ပြီး git repository ကို ပြန်လည် ဒေါင်းလုဒ်လုပ်ပါ။

## လင့်ခ်များ (Links)

-   Workbench Wiki:
-   FreeCAD Wiki:
-   FreeCAD Forum: <http://forum.freecadweb.org/viewtopic.php?f=10&t=8577>
-   Tutorials:
-   Videos: [video 1](https://www.youtube.com/watch?v=dhaYJKDk4GI), [video 2](http://youtu.be/ufhyUxQkeC0),
-   Files:
-   Report bugs: အမှားတွေ့ပါက ကျေးဇူးပြု၍ <https://github.com/hamish2014/FreeCAD_assembly2/issues> တွင် အစီရင်ခံပါ။

## အခြား အသုံးဝင် လင့်ခ်များ

-   [Animation](http://www.freecadweb.org/wiki/index.php?title=Sandbox:Animation): ဤ လုပ်ငန်းခွင်ကို ပုံရ sequence များ ဖန်တီးရန် အသုံးပြုနိုင်သည်။
-   [ExplodedAnimation](http://www.freecadweb.org/wiki/index.php?title=Sandbox:ExplodedAnimation): assembly များ၏ exploded view နှင့် animation များ ဖန်တီးရန် FreeCAD လုပ်ငန်းခွင်။
-   [External workbenches](External_workbenches.md)



---
⏵ [documentation index](../README.md) > [User Documentation](Category_User%20Documentation.md) > [Addons](Category_Addons.md) > [External Workbenches](Category_External%20Workbenches.md) > Assembly2 လုပ်ငန်းခွင် (Workbench)