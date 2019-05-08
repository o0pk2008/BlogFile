---
title: UE4_透明线框材质效果实现
date: 2019-04-10 11:41:56
tags: UE4_Material
categories: UnrealEngine4
---
![最终效果](UE4_01.jpg)

材质蓝图
<iframe frameborder="no" border="0" width="100%" height="600" src="https://blueprintue.com/render/7ideosxm" scrolling="no"></iframe>

{% codeblock 材质代码 %}
Begin Object Class=/Script/UnrealEd.MaterialGraphNode_Root Name="MaterialGraphNode_Root_0"
   Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   NodePosX=-16
   NodeGuid=8612B9F24539DF565282858AE9E02E73
   CustomProperties Pin (PinId=9971543842C10196DDAFC38AF1836A3C,PinName="Base Color",PinType.PinCategory="materialinput",PinType.PinSubCategory="5",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 FD84F46E43B65C555806429D19DE050C,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=92A716584B08A6D6818912B151BBC016,PinName="Metallic",PinType.PinCategory="materialinput",PinType.PinSubCategory="6",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=0D7ADF404146471BDE7ECE9310818D2F,PinName="Specular",PinType.PinCategory="materialinput",PinType.PinSubCategory="7",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=015AC9FA496E3968936A8FB37A980CEA,PinName="Roughness",PinType.PinCategory="materialinput",PinType.PinSubCategory="8",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=89CF09E54BC30E2266C6C2AF03B0BC56,PinName="Emissive Color",PinType.PinCategory="materialinput",PinType.PinSubCategory="0",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 FD84F46E43B65C555806429D19DE050C,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=B1F07CC9484AFCDAA9B70986670365A2,PinName="Opacity",PinType.PinCategory="materialinput",PinType.PinSubCategory="1",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_1 A769F6FF43177118E40555A0DAFE1496,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=7B3D13D145D14A769C82038B5288D4AB,PinName="Opacity Mask",PinType.PinCategory="materialinput",PinType.PinSubCategory="2",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=72CF7E6D4001B378B907ECA810D601EC,PinName="Normal",PinType.PinCategory="materialinput",PinType.PinSubCategory="9",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=07EAB04C489607AAA0E43DAB436CF90F,PinName="World Position Offset",PinType.PinCategory="materialinput",PinType.PinSubCategory="10",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=DDACE15C4618DBF34C8BDDBE4622ED3D,PinName="World Displacement",PinType.PinCategory="materialinput",PinType.PinSubCategory="11",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=53E904DE43AAEFA713037381403F83DC,PinName="Tessellation Multiplier",PinType.PinCategory="materialinput",PinType.PinSubCategory="12",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=30590DA64FC97BE8CAF3C7AB6EC1107E,PinName="Subsurface Color",PinType.PinCategory="materialinput",PinType.PinSubCategory="13",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=014054E941B97DAB06DD3DAA143B826E,PinName="Custom Data 0",PinType.PinCategory="materialinput",PinType.PinSubCategory="14",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=F2ADB5544B3FEE8C3230489AF44E6201,PinName="Custom Data 1",PinType.PinCategory="materialinput",PinType.PinSubCategory="15",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=93B4C24A41D33BB0350F778C68DCE494,PinName="Ambient Occlusion",PinType.PinCategory="materialinput",PinType.PinSubCategory="16",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=42A39A5443844549838CCFAA80A98B54,PinName="Refraction",PinType.PinCategory="materialinput",PinType.PinSubCategory="17",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=BD3179C7441464AAE48828B80AA8569A,PinName="Customized UV0",PinType.PinCategory="materialinput",PinType.PinSubCategory="18",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=4FC42FDF43DA469CF036BDA1A63C1121,PinName="Customized UV1",PinType.PinCategory="materialinput",PinType.PinSubCategory="19",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=25DED0A04BB18045ADCD2B91D67363A2,PinName="Customized UV2",PinType.PinCategory="materialinput",PinType.PinSubCategory="20",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=92BFFE8B45251579A97383BDDF5F5383,PinName="Customized UV3",PinType.PinCategory="materialinput",PinType.PinSubCategory="21",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=DEE6963B430794F035BBE69DFDD0FCBC,PinName="Customized UV4",PinType.PinCategory="materialinput",PinType.PinSubCategory="22",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=49587C6D44C1A72A27753482136A7812,PinName="Customized UV5",PinType.PinCategory="materialinput",PinType.PinSubCategory="23",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=C1E0D31743FFFE6E2FDA829C68FA3095,PinName="Customized UV6",PinType.PinCategory="materialinput",PinType.PinSubCategory="24",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=2466B2D0461EA88908EB34B35FC28452,PinName="Customized UV7",PinType.PinCategory="materialinput",PinType.PinSubCategory="25",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D7B1254C43CB1E807CC296AE36124BC7,PinName="Pixel Depth Offset",PinType.PinCategory="materialinput",PinType.PinSubCategory="26",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=169BB3A246878C743C6B99BDCF2138D3,PinName="Material Attributes",PinType.PinCategory="materialinput",PinType.PinSubCategory="27",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_0"
   Begin Object Class=/Script/Engine.MaterialExpressionMultiply Name="MaterialExpressionMultiply_0"
   End Object
   Begin Object Name="MaterialExpressionMultiply_0"
      A=(Expression=MaterialExpressionLinearInterpolate'"MaterialGraphNode_8.MaterialExpressionLinearInterpolate_3"')
      B=(Expression=MaterialExpressionConstant3Vector'"MaterialGraphNode_12.MaterialExpressionConstant3Vector_6"')
      MaterialExpressionEditorX=-288
      MaterialExpressionEditorY=96
      MaterialExpressionGuid=F1C8D1344715FD58D9C434B40F3068BC
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionMultiply'"MaterialExpressionMultiply_0"'
   NodePosX=-288
   NodePosY=96
   NodeGuid=28A1948C49D6586163C305A6AFFFB50F
   CustomProperties Pin (PinId=3726D0F64F60C2BF601DB985253E7B05,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_8 18706D5B4707FDD1D3120AAF5D183A31,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=AEA5DE4646D5A22F0F456BA7EBD0916C,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_12 95BD76AE440C658FFB0A4693F697DE86,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=FD84F46E43B65C555806429D19DE050C,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_Root_0 9971543842C10196DDAFC38AF1836A3C,MaterialGraphNode_Root_0 89CF09E54BC30E2266C6C2AF03B0BC56,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_1"
   Begin Object Class=/Script/Engine.MaterialExpressionLinearInterpolate Name="MaterialExpressionLinearInterpolate_4"
   End Object
   Begin Object Name="MaterialExpressionLinearInterpolate_4"
      A=(Expression=MaterialExpressionConstant'"MaterialGraphNode_9.MaterialExpressionConstant_3"')
      B=(Expression=MaterialExpressionFresnel'"MaterialGraphNode_10.MaterialExpressionFresnel_2"')
      Alpha=(Expression=MaterialExpressionIf'"MaterialGraphNode_4.MaterialExpressionIf_0"')
      MaterialExpressionEditorX=-464
      MaterialExpressionEditorY=352
      MaterialExpressionGuid=821C2E2547DF6C00CEC5628AA3137408
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionLinearInterpolate'"MaterialExpressionLinearInterpolate_4"'
   NodePosX=-464
   NodePosY=352
   NodeGuid=8901AE1C4FACEA282528979F520EE136
   CustomProperties Pin (PinId=F319316048ADA841C1FB939926D20A33,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_9 971BAAB641CF3A16D8872086487F2090,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=25C052DD4DB15673EE537F98B97A5BB8,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_10 6F88FE2549522A42F1C52CAADAD79A09,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=4817E9A4451E339FBB85BD8E6DBED9AC,PinName="Alpha",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 4C47AB1246F3D6A6AF894E804368C5BC,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=A769F6FF43177118E40555A0DAFE1496,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_Root_0 B1F07CC9484AFCDAA9B70986670365A2,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_2"
   Begin Object Class=/Script/Engine.MaterialExpressionWorldPosition Name="MaterialExpressionWorldPosition_0"
   End Object
   Begin Object Name="MaterialExpressionWorldPosition_0"
      MaterialExpressionEditorX=-1232
      MaterialExpressionEditorY=304
      MaterialExpressionGuid=824B280E41504D7C63128B9E9272B402
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionWorldPosition'"MaterialExpressionWorldPosition_0"'
   NodePosX=-1232
   NodePosY=304
   NodeGuid=3CB735C145B134CCE737F9952EF8BD82
   CustomProperties Pin (PinId=CA360CB54052210299FB33970A3C4BFA,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_3 03A4F0E443C9C6B0B10A4F9893A5D44F,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_3"
   Begin Object Class=/Script/Engine.MaterialExpressionComponentMask Name="MaterialExpressionComponentMask_0"
   End Object
   Begin Object Name="MaterialExpressionComponentMask_0"
      Input=(Expression=MaterialExpressionWorldPosition'"MaterialGraphNode_2.MaterialExpressionWorldPosition_0"')
      B=True
      MaterialExpressionEditorX=-1024
      MaterialExpressionEditorY=320
      MaterialExpressionGuid=C0DEFF714B8DAED3EEF4558B3272AB9A
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionComponentMask'"MaterialExpressionComponentMask_0"'
   NodePosX=-1024
   NodePosY=320
   NodeGuid=69DDCA774BD777AE6A520D8B75538639
   CustomProperties Pin (PinId=03A4F0E443C9C6B0B10A4F9893A5D44F,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_2 CA360CB54052210299FB33970A3C4BFA,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=889289D044131DA97B1986906E2F239C,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 428FDF564BA3FB43C6DDC1B179167F4E,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_4"
   Begin Object Class=/Script/Engine.MaterialExpressionIf Name="MaterialExpressionIf_0"
   End Object
   Begin Object Name="MaterialExpressionIf_0"
      A=(Expression=MaterialExpressionComponentMask'"MaterialGraphNode_3.MaterialExpressionComponentMask_0"')
      B=(Expression=MaterialExpressionConstant'"MaterialGraphNode_5.MaterialExpressionConstant_0"')
      AGreaterThanB=(Expression=MaterialExpressionConstant'"MaterialGraphNode_6.MaterialExpressionConstant_1"')
      AEqualsB=(Expression=MaterialExpressionConstant'"MaterialGraphNode_6.MaterialExpressionConstant_1"')
      ALessThanB=(Expression=MaterialExpressionConstant'"MaterialGraphNode_7.MaterialExpressionConstant_2"')
      MaterialExpressionEditorX=-880
      MaterialExpressionEditorY=320
      MaterialExpressionGuid=8536396C474FFC002B1F308076BFCE2B
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionIf'"MaterialExpressionIf_0"'
   NodePosX=-880
   NodePosY=320
   NodeGuid=524D9AE44A888BCD51216BB0ECA39440
   CustomProperties Pin (PinId=428FDF564BA3FB43C6DDC1B179167F4E,PinName="A",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_3 889289D044131DA97B1986906E2F239C,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=870DDA6348855C970933ED8981C7C5D5,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_5 7CF5394A4CDF24A7297DA592ACD58AAF,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=E8FA8CBA4F185895E0E46086CE4FDA8B,PinName="A > B",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_6 D8D141084C45AEBCF12E529393911DFD,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=33447E6E4E04B76625F45DA0541A7334,PinName="A == B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_6 D8D141084C45AEBCF12E529393911DFD,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=ED0EC66940D237C17008C8B3529AE8E4,PinName="A < B",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_7 A43CB09E4D26714BD06DE6B5DC90DDD0,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=4C47AB1246F3D6A6AF894E804368C5BC,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_1 4817E9A4451E339FBB85BD8E6DBED9AC,MaterialGraphNode_8 3FF3C88244C5E501474A87A168EE1095,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_5"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant Name="MaterialExpressionConstant_0"
   End Object
   Begin Object Name="MaterialExpressionConstant_0"
      R=18.000000
      MaterialExpressionEditorX=-1104
      MaterialExpressionEditorY=384
      MaterialExpressionGuid=7B0E81EE4D0767764BF4A681A63B945E
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionConstant'"MaterialExpressionConstant_0"'
   NodePosX=-1104
   NodePosY=384
   NodeGuid=3C3420BD4B503A972C40BCA439D4F3F0
   CustomProperties Pin (PinId=7CF5394A4CDF24A7297DA592ACD58AAF,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 870DDA6348855C970933ED8981C7C5D5,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_6"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant Name="MaterialExpressionConstant_1"
   End Object
   Begin Object Name="MaterialExpressionConstant_1"
      R=1.000000
      MaterialExpressionEditorX=-1120
      MaterialExpressionEditorY=464
      MaterialExpressionGuid=5E5A1BC34DA7095FA5E06AA11FA939CF
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionConstant'"MaterialExpressionConstant_1"'
   NodePosX=-1120
   NodePosY=464
   NodeGuid=1FCC15B04BE8A3A367ED1ABEE11DFA5E
   CustomProperties Pin (PinId=D8D141084C45AEBCF12E529393911DFD,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 E8FA8CBA4F185895E0E46086CE4FDA8B,MaterialGraphNode_4 33447E6E4E04B76625F45DA0541A7334,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_7"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant Name="MaterialExpressionConstant_2"
   End Object
   Begin Object Name="MaterialExpressionConstant_2"
      MaterialExpressionEditorX=-1120
      MaterialExpressionEditorY=528
      MaterialExpressionGuid=1786F71D43553AE70246E98EC3928110
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionConstant'"MaterialExpressionConstant_2"'
   NodePosX=-1120
   NodePosY=528
   NodeGuid=7220447640F02DA7B778D69F3272B493
   CustomProperties Pin (PinId=A43CB09E4D26714BD06DE6B5DC90DDD0,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 ED0EC66940D237C17008C8B3529AE8E4,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_8"
   Begin Object Class=/Script/Engine.MaterialExpressionLinearInterpolate Name="MaterialExpressionLinearInterpolate_3"
   End Object
   Begin Object Name="MaterialExpressionLinearInterpolate_3"
      A=(Expression=MaterialExpressionConstant3Vector'"MaterialGraphNode_11.MaterialExpressionConstant3Vector_5"')
      B=(Expression=MaterialExpressionConstant3Vector'"MaterialGraphNode_12.MaterialExpressionConstant3Vector_6"')
      Alpha=(Expression=MaterialExpressionIf'"MaterialGraphNode_4.MaterialExpressionIf_0"')
      MaterialExpressionEditorX=-480
      MaterialExpressionEditorY=-16
      MaterialExpressionGuid=821C2E2547DF6C00CEC5628AA3137408
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionLinearInterpolate'"MaterialExpressionLinearInterpolate_3"'
   NodePosX=-480
   NodePosY=-16
   NodeGuid=75835E484F073B51F930E181DB6BEBA2
   CustomProperties Pin (PinId=6F7AF8D144554E3CBF1EBEA92D95DA6F,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_11 B76E719C437C64398BFF2383BADF541B,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D8B31A504A042C4F0C84DCB4BC0293F2,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_12 95BD76AE440C658FFB0A4693F697DE86,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=3FF3C88244C5E501474A87A168EE1095,PinName="Alpha",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 4C47AB1246F3D6A6AF894E804368C5BC,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=18706D5B4707FDD1D3120AAF5D183A31,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 3726D0F64F60C2BF601DB985253E7B05,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_9"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant Name="MaterialExpressionConstant_3"
   End Object
   Begin Object Name="MaterialExpressionConstant_3"
      R=1.000000
      MaterialExpressionEditorX=-560
      MaterialExpressionEditorY=352
      MaterialExpressionGuid=DC483C604612452344D5439D3DD3A87E
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionConstant'"MaterialExpressionConstant_3"'
   NodePosX=-560
   NodePosY=352
   NodeGuid=27F0697847D8EF7F7B8282B6F3A97A0A
   CustomProperties Pin (PinId=971BAAB641CF3A16D8872086487F2090,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_1 F319316048ADA841C1FB939926D20A33,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_10"
   Begin Object Class=/Script/Engine.MaterialExpressionFresnel Name="MaterialExpressionFresnel_2"
   End Object
   Begin Object Name="MaterialExpressionFresnel_2"
      MaterialExpressionEditorX=-704
      MaterialExpressionEditorY=432
      MaterialExpressionGuid=26B02637493331B1C60F42B633E69B51
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionFresnel'"MaterialExpressionFresnel_2"'
   NodePosX=-704
   NodePosY=432
   NodeGuid=944AF1EE47977C8A6D78D187A4916A78
   CustomProperties Pin (PinId=70973C794E2C4E7FEC3545B02F17804D,PinName="ExponentIn",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=85D64B774EB329986CB472875E28C0F9,PinName="BaseReflectFractionIn",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=CD567BAD4913531F127FE6BBA1590A94,PinName="Normal",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=6F88FE2549522A42F1C52CAADAD79A09,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_1 25C052DD4DB15673EE537F98B97A5BB8,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_11"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant3Vector Name="MaterialExpressionConstant3Vector_5"
   End Object
   Begin Object Name="MaterialExpressionConstant3Vector_5"
      Constant=(R=0.000000,G=0.007060,B=0.050000,A=0.000000)
      MaterialExpressionEditorX=-672
      MaterialExpressionEditorY=-16
      MaterialExpressionGuid=1ACF9FE442D28499A184F1819CE21803
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionConstant3Vector'"MaterialExpressionConstant3Vector_5"'
   NodePosX=-672
   NodePosY=-16
   NodeGuid=7A9732AF4F89C395CF9149B500320FEC
   CustomProperties Pin (PinId=B76E719C437C64398BFF2383BADF541B,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_8 6F7AF8D144554E3CBF1EBEA92D95DA6F,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_12"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant3Vector Name="MaterialExpressionConstant3Vector_6"
   End Object
   Begin Object Name="MaterialExpressionConstant3Vector_6"
      Constant=(R=0.090400,G=0.642000,B=1.000000,A=0.000000)
      MaterialExpressionEditorX=-672
      MaterialExpressionEditorY=144
      MaterialExpressionGuid=EF4C1B44430DED2FA7E7839A4816353E
      Material=PreviewMaterial'"/Engine/Transient.M_Blue"'
   End Object
   MaterialExpression=MaterialExpressionConstant3Vector'"MaterialExpressionConstant3Vector_6"'
   NodePosX=-672
   NodePosY=144
   NodeGuid=E548F6C64945F19B315070B69DDB9230
   CustomProperties Pin (PinId=95BD76AE440C658FFB0A4693F697DE86,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 AEA5DE4646D5A22F0F456BA7EBD0916C,MaterialGraphNode_8 D8B31A504A042C4F0C84DCB4BC0293F2,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object

{% endcodeblock %}

![参数设置](UE4_02.jpg)