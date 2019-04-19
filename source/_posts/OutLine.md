---
title: OutLine
date: 2019-04-11 15:07:16
tags: UE4_Material
categories: UnrealEngine4
---

![最终效果](01.jpg)
{% codeblock 材质代码 %}
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_0"
   Begin Object Class=/Script/Engine.MaterialExpressionLinearInterpolate Name="MaterialExpressionLinearInterpolate_0"
   End Object
   Begin Object Name="MaterialExpressionLinearInterpolate_0"
      A=(Expression=MaterialExpressionSceneTexture'"MaterialGraphNode_38.MaterialExpressionSceneTexture_0"',Mask=1,MaskR=1,MaskG=1,MaskB=1,MaskA=1)
      B=(Expression=MaterialExpressionAppendVector'"MaterialGraphNode_32.MaterialExpressionAppendVector_4"')
      Alpha=(Expression=MaterialExpressionMultiply'"MaterialGraphNode_34.MaterialExpressionMultiply_2"')
      MaterialExpressionEditorX=-640
      MaterialExpressionEditorY=64
      MaterialExpressionGuid=4E48C8CE49C3E8F29C7326ADE1ADF29E
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionLinearInterpolate'"MaterialExpressionLinearInterpolate_0"'
   NodePosX=-640
   NodePosY=64
   NodeGuid=069E3FCC42BEF360DD4FC79128116792
   CustomProperties Pin (PinId=3EF0ADDF427C6243CF105D9BEC7098F1,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_38 5ADD66E44050C33664C4A5986B2382A4,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=8DDD282B4F80588BFE5E86A9A74283B2,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_32 F9AC305444B7B31BF04F86961991C7C7,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=C410ED8C467745FE48E45C853A545951,PinName="Alpha",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_34 06EB87624354CFEA0424488E4A9BFD02,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=32325C7B437B9E07BE7371A6AFE4FAC6,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_Root_0 467DE0EB4EC225ED9B1A2FABE2F55817,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_1"
   Begin Object Class=/Script/Engine.MaterialExpressionSceneTexelSize Name="MaterialExpressionSceneTexelSize_0"
   End Object
   Begin Object Name="MaterialExpressionSceneTexelSize_0"
      MaterialExpressionEditorX=-3056
      MaterialExpressionEditorY=368
      MaterialExpressionGuid=1F1D3BF4485FA5867E3F23B490413697
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSceneTexelSize'"MaterialExpressionSceneTexelSize_0"'
   NodePosX=-3056
   NodePosY=368
   NodeGuid=0AF31A8D408F92283CAF36BEF121B791
   CustomProperties Pin (PinId=67CD77AE4D684121B0E33CADCD6F1A62,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_3 104928C740D9B57F3B099BB346026C3F,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_2"
   Begin Object Class=/Script/Engine.MaterialExpressionScalarParameter Name="MaterialExpressionScalarParameter_0"
   End Object
   Begin Object Name="MaterialExpressionScalarParameter_0"
      DefaultValue=1.000000
      ParameterName="OutlineWidth"
      ExpressionGUID=73F36FF041723C7AA098D19D5EDFC92A
      MaterialExpressionEditorX=-3040
      MaterialExpressionEditorY=480
      MaterialExpressionGuid=75020D724ACBE2D15A0745AB81A46BBE
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionScalarParameter'"MaterialExpressionScalarParameter_0"'
   NodePosX=-3040
   NodePosY=480
   bCanRenameNode=True
   NodeGuid=CF4F0D664C9B8CA8288230A63A253501
   CustomProperties Pin (PinId=E7C1B33341D29A643227FC8FBAD33025,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_3 01D95A954B92BBBF21528593836E0295,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_3"
   Begin Object Class=/Script/Engine.MaterialExpressionMultiply Name="MaterialExpressionMultiply_0"
   End Object
   Begin Object Name="MaterialExpressionMultiply_0"
      A=(Expression=MaterialExpressionSceneTexelSize'"MaterialGraphNode_1.MaterialExpressionSceneTexelSize_0"')
      B=(Expression=MaterialExpressionScalarParameter'"MaterialGraphNode_2.MaterialExpressionScalarParameter_0"')
      MaterialExpressionEditorX=-2880
      MaterialExpressionEditorY=416
      MaterialExpressionGuid=1DE37CF94AC88FAE9D8854AB01937AEC
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionMultiply'"MaterialExpressionMultiply_0"'
   NodePosX=-2880
   NodePosY=416
   NodeGuid=8F2F54D54D4700F5D92ABDA97490659E
   CustomProperties Pin (PinId=104928C740D9B57F3B099BB346026C3F,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_1 67CD77AE4D684121B0E33CADCD6F1A62,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=01D95A954B92BBBF21528593836E0295,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_2 E7C1B33341D29A643227FC8FBAD33025,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=3AE7C1ED43E914869B68D4A8A8AFBDD8,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 E5C2B64E4EA4603C2855F6A7992C1EB8,MaterialGraphNode_5 A9A6E5E448B79629C66F7F8C17A88564,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_4"
   Begin Object Class=/Script/Engine.MaterialExpressionComponentMask Name="MaterialExpressionComponentMask_0"
   End Object
   Begin Object Name="MaterialExpressionComponentMask_0"
      Input=(Expression=MaterialExpressionMultiply'"MaterialGraphNode_3.MaterialExpressionMultiply_0"')
      R=True
      MaterialExpressionEditorX=-2704
      MaterialExpressionEditorY=336
      MaterialExpressionGuid=73FC7D72434BE95226F8849E8F0F575F
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionComponentMask'"MaterialExpressionComponentMask_0"'
   NodePosX=-2704
   NodePosY=336
   NodeGuid=F4575D8B45CE8347353F2DB554738873
   CustomProperties Pin (PinId=E5C2B64E4EA4603C2855F6A7992C1EB8,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_3 3AE7C1ED43E914869B68D4A8A8AFBDD8,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=434D99914A209D0896B0D392DC1944EA,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_6 930EB60A45286FA5FCC4A99B5847A4F1,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_5"
   Begin Object Class=/Script/Engine.MaterialExpressionComponentMask Name="MaterialExpressionComponentMask_1"
   End Object
   Begin Object Name="MaterialExpressionComponentMask_1"
      Input=(Expression=MaterialExpressionMultiply'"MaterialGraphNode_3.MaterialExpressionMultiply_0"')
      G=True
      MaterialExpressionEditorX=-2704
      MaterialExpressionEditorY=576
      MaterialExpressionGuid=9BA4D25D4E5E5ACD3AE9BC9033BF49A7
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionComponentMask'"MaterialExpressionComponentMask_1"'
   NodePosX=-2704
   NodePosY=576
   NodeGuid=F294A9C248C6C912BDE38191CD28FA07
   CustomProperties Pin (PinId=A9A6E5E448B79629C66F7F8C17A88564,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_3 3AE7C1ED43E914869B68D4A8A8AFBDD8,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=5484C6E1458A1DADF8C711A050AB16CA,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_8 B1426584417CEFE23A43CD8DD9CCB4B3,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_6"
   Begin Object Class=/Script/Engine.MaterialExpressionAppendVector Name="MaterialExpressionAppendVector_0"
   End Object
   Begin Object Name="MaterialExpressionAppendVector_0"
      A=(Expression=MaterialExpressionComponentMask'"MaterialGraphNode_4.MaterialExpressionComponentMask_0"')
      B=(Expression=MaterialExpressionConstant'"MaterialGraphNode_7.MaterialExpressionConstant_1"')
      MaterialExpressionEditorX=-2512
      MaterialExpressionEditorY=336
      MaterialExpressionGuid=94F22D1348A2F23111FDFF907322A6B4
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAppendVector'"MaterialExpressionAppendVector_0"'
   NodePosX=-2512
   NodePosY=336
   NodeGuid=6C24B900435E0E3D4C0963AACF85CF82
   CustomProperties Pin (PinId=930EB60A45286FA5FCC4A99B5847A4F1,PinName="A",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_4 434D99914A209D0896B0D392DC1944EA,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=A02B464546756D921A6656BCE9517518,PinName="B",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_7 0E8738BF49C0FF0DF28F7A93FF0B3FF5,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=5B19271C4A5D3CE7BF7804B64E1A7801,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_10 D2C4B59F41B49AE1EE19E5A303E06313,MaterialGraphNode_11 067F41FC4406A6761D616C8A252C9D30,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_7"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant Name="MaterialExpressionConstant_1"
   End Object
   Begin Object Name="MaterialExpressionConstant_1"
      MaterialExpressionEditorX=-2656
      MaterialExpressionEditorY=448
      MaterialExpressionGuid=FA5F1D504A17ACBCB8A2C5B36CD0DD3A
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionConstant'"MaterialExpressionConstant_1"'
   NodePosX=-2656
   NodePosY=448
   NodeGuid=E7572EC74CCC66D542C70E9790BA6DD5
   CustomProperties Pin (PinId=0E8738BF49C0FF0DF28F7A93FF0B3FF5,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_6 A02B464546756D921A6656BCE9517518,MaterialGraphNode_8 7ADC824B47FE8E82C459E9ADC9E338FC,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_8"
   Begin Object Class=/Script/Engine.MaterialExpressionAppendVector Name="MaterialExpressionAppendVector_1"
   End Object
   Begin Object Name="MaterialExpressionAppendVector_1"
      A=(Expression=MaterialExpressionConstant'"MaterialGraphNode_7.MaterialExpressionConstant_1"')
      B=(Expression=MaterialExpressionComponentMask'"MaterialGraphNode_5.MaterialExpressionComponentMask_1"')
      MaterialExpressionEditorX=-2512
      MaterialExpressionEditorY=544
      MaterialExpressionGuid=CC2DE4F64EC5D574C1F1F9A81FFD049C
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAppendVector'"MaterialExpressionAppendVector_1"'
   NodePosX=-2512
   NodePosY=544
   NodeGuid=0096137B479E8C400D305FAE4E576C0A
   CustomProperties Pin (PinId=7ADC824B47FE8E82C459E9ADC9E338FC,PinName="A",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_7 0E8738BF49C0FF0DF28F7A93FF0B3FF5,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=B1426584417CEFE23A43CD8DD9CCB4B3,PinName="B",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_5 5484C6E1458A1DADF8C711A050AB16CA,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=2C5DBD5542476FBCACF34986FE9CA820,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_12 23C6B8B3453F623AF0C4F3AC5283AB9D,MaterialGraphNode_13 012AD2924DCF9A273A0E8B989D2E6A0D,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_9"
   Begin Object Class=/Script/Engine.MaterialExpressionScreenPosition Name="MaterialExpressionScreenPosition_0"
   End Object
   Begin Object Name="MaterialExpressionScreenPosition_0"
      MaterialExpressionEditorX=-2496
      MaterialExpressionEditorY=448
      MaterialExpressionGuid=DD76017E41074F61B2740E9FBCD81AEE
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionScreenPosition'"MaterialExpressionScreenPosition_0"'
   NodePosX=-2496
   NodePosY=448
   NodeGuid=3FE5F6844F000A9536DA60812808C296
   CustomProperties Pin (PinId=5157534C4EA234E71E7A04B683631BDD,PinName="ViewportUV",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_10 D411BFC44B55D9944BA125A506D5AAD5,MaterialGraphNode_11 774F47524CB8CC8B67E39CBE26EA6C3D,MaterialGraphNode_12 A9538EAF4B48617F8A0B3BBAC5A5998F,MaterialGraphNode_13 3BBED18A4CDD2B59A3304BA4177806D1,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=2EF91401453737062B5D96B4B442A114,PinName="PixelPosition",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_10"
   Begin Object Class=/Script/Engine.MaterialExpressionAdd Name="MaterialExpressionAdd_0"
   End Object
   Begin Object Name="MaterialExpressionAdd_0"
      A=(Expression=MaterialExpressionAppendVector'"MaterialGraphNode_6.MaterialExpressionAppendVector_0"')
      B=(Expression=MaterialExpressionScreenPosition'"MaterialGraphNode_9.MaterialExpressionScreenPosition_0"')
      MaterialExpressionEditorX=-2224
      MaterialExpressionEditorY=256
      MaterialExpressionGuid=8FF5C4D943B1D50D48980BBA92CB9C79
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAdd'"MaterialExpressionAdd_0"'
   NodePosX=-2224
   NodePosY=256
   NodeGuid=F38E1B7643DAC39213178D836F52EE92
   CustomProperties Pin (PinId=D2C4B59F41B49AE1EE19E5A303E06313,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_6 5B19271C4A5D3CE7BF7804B64E1A7801,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D411BFC44B55D9944BA125A506D5AAD5,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_9 5157534C4EA234E71E7A04B683631BDD,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=EAF87BA0403F50A0B4B2A3AB7A7510B3,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_14 FA74B85746F23BA79E89B5B4145A9A49,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_11"
   Begin Object Class=/Script/Engine.MaterialExpressionSubtract Name="MaterialExpressionSubtract_0"
   End Object
   Begin Object Name="MaterialExpressionSubtract_0"
      A=(Expression=MaterialExpressionScreenPosition'"MaterialGraphNode_9.MaterialExpressionScreenPosition_0"')
      B=(Expression=MaterialExpressionAppendVector'"MaterialGraphNode_6.MaterialExpressionAppendVector_0"')
      MaterialExpressionEditorX=-2224
      MaterialExpressionEditorY=368
      MaterialExpressionGuid=0369388940B56A813D23FBBDA906E2AE
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSubtract'"MaterialExpressionSubtract_0"'
   NodePosX=-2224
   NodePosY=368
   NodeGuid=F872DEAA497FCED282665CA749EF9615
   CustomProperties Pin (PinId=774F47524CB8CC8B67E39CBE26EA6C3D,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_9 5157534C4EA234E71E7A04B683631BDD,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=067F41FC4406A6761D616C8A252C9D30,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_6 5B19271C4A5D3CE7BF7804B64E1A7801,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=8945EF7C494B58BA358332BF050153E2,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_15 E6C881C74D55C31C987758B4D7A8355A,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_12"
   Begin Object Class=/Script/Engine.MaterialExpressionAdd Name="MaterialExpressionAdd_1"
   End Object
   Begin Object Name="MaterialExpressionAdd_1"
      A=(Expression=MaterialExpressionScreenPosition'"MaterialGraphNode_9.MaterialExpressionScreenPosition_0"')
      B=(Expression=MaterialExpressionAppendVector'"MaterialGraphNode_8.MaterialExpressionAppendVector_1"')
      MaterialExpressionEditorX=-2224
      MaterialExpressionEditorY=480
      MaterialExpressionGuid=66402CC7454510BEF7DC2594959A0C5C
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAdd'"MaterialExpressionAdd_1"'
   NodePosX=-2224
   NodePosY=480
   NodeGuid=E4983F3E4CF037A042FCC0843CA4239C
   CustomProperties Pin (PinId=A9538EAF4B48617F8A0B3BBAC5A5998F,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_9 5157534C4EA234E71E7A04B683631BDD,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=23C6B8B3453F623AF0C4F3AC5283AB9D,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_8 2C5DBD5542476FBCACF34986FE9CA820,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=7C8EC69C409BD048AC7A4CB34A3AE1E6,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_16 586CF3C94E9D6D084B985787ED645EA1,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_13"
   Begin Object Class=/Script/Engine.MaterialExpressionSubtract Name="MaterialExpressionSubtract_1"
   End Object
   Begin Object Name="MaterialExpressionSubtract_1"
      A=(Expression=MaterialExpressionScreenPosition'"MaterialGraphNode_9.MaterialExpressionScreenPosition_0"')
      B=(Expression=MaterialExpressionAppendVector'"MaterialGraphNode_8.MaterialExpressionAppendVector_1"')
      MaterialExpressionEditorX=-2224
      MaterialExpressionEditorY=592
      MaterialExpressionGuid=874CB3E444A0D418B6D61BB6F1ABE9C0
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSubtract'"MaterialExpressionSubtract_1"'
   NodePosX=-2224
   NodePosY=592
   NodeGuid=D8E4947E414C2E7A80E924A2C169DADE
   CustomProperties Pin (PinId=3BBED18A4CDD2B59A3304BA4177806D1,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_9 5157534C4EA234E71E7A04B683631BDD,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=012AD2924DCF9A273A0E8B989D2E6A0D,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_8 2C5DBD5542476FBCACF34986FE9CA820,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D2CF074D4EA63DD5048B2D8017914365,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_17 9839044345A55C546CA1208741682648,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_14"
   Begin Object Class=/Script/Engine.MaterialExpressionSceneTexture Name="MaterialExpressionSceneTexture_3"
   End Object
   Begin Object Name="MaterialExpressionSceneTexture_3"
      Coordinates=(Expression=MaterialExpressionAdd'"MaterialGraphNode_10.MaterialExpressionAdd_0"')
      SceneTextureId=PPI_CustomDepth
      MaterialExpressionEditorX=-2032
      MaterialExpressionEditorY=192
      MaterialExpressionGuid=52F8C7DD43D02DC47162F3BB4FFA7355
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSceneTexture'"MaterialExpressionSceneTexture_3"'
   NodePosX=-2032
   NodePosY=192
   NodeGuid=9228EE7540427BFD0E68759C33FE7CCB
   CustomProperties Pin (PinId=FA74B85746F23BA79E89B5B4145A9A49,PinName="UVs",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_10 EAF87BA0403F50A0B4B2A3AB7A7510B3,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=05090A1E4497156685AD89B66691764C,PinName="Color",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="rgba",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_18 66D013F44AC2019514616294114E7308,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=E9D803BC4D75E65CC0C5CD823D633A1D,PinName="Size",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D88977F64013B7D34307B18E7B9D849E,PinName="InvSize",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_15"
   Begin Object Class=/Script/Engine.MaterialExpressionSceneTexture Name="MaterialExpressionSceneTexture_6"
   End Object
   Begin Object Name="MaterialExpressionSceneTexture_6"
      Coordinates=(Expression=MaterialExpressionSubtract'"MaterialGraphNode_11.MaterialExpressionSubtract_0"')
      SceneTextureId=PPI_CustomDepth
      MaterialExpressionEditorX=-2032
      MaterialExpressionEditorY=352
      MaterialExpressionGuid=52F8C7DD43D02DC47162F3BB4FFA7355
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSceneTexture'"MaterialExpressionSceneTexture_6"'
   NodePosX=-2032
   NodePosY=352
   NodeGuid=866945304E7D1B237B6AC6A18CB1E84C
   CustomProperties Pin (PinId=E6C881C74D55C31C987758B4D7A8355A,PinName="UVs",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_11 8945EF7C494B58BA358332BF050153E2,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=46FD58604FF29C181BB579B66B265E70,PinName="Color",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="rgba",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_18 0EAD1630472F82BBB0FE2ABFB7B729A6,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=21F47BCA4F8FB6EBCA178E9D77318258,PinName="Size",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=DE94408040661894B53E29986697E3B1,PinName="InvSize",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_16"
   Begin Object Class=/Script/Engine.MaterialExpressionSceneTexture Name="MaterialExpressionSceneTexture_7"
   End Object
   Begin Object Name="MaterialExpressionSceneTexture_7"
      Coordinates=(Expression=MaterialExpressionAdd'"MaterialGraphNode_12.MaterialExpressionAdd_1"')
      SceneTextureId=PPI_CustomDepth
      MaterialExpressionEditorX=-2032
      MaterialExpressionEditorY=496
      MaterialExpressionGuid=52F8C7DD43D02DC47162F3BB4FFA7355
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSceneTexture'"MaterialExpressionSceneTexture_7"'
   NodePosX=-2032
   NodePosY=496
   NodeGuid=8A52E66D450E2F7272E009B5C249AF23
   CustomProperties Pin (PinId=586CF3C94E9D6D084B985787ED645EA1,PinName="UVs",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_12 7C8EC69C409BD048AC7A4CB34A3AE1E6,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=45826F9E408895666B856E9953EB1773,PinName="Color",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="rgba",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_19 AF143D5D49782637C4998C836280D3FA,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=8C4130C54A7418697BC91A921710C38B,PinName="Size",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=68CE3003479E0C19D4B0099C42FBE8C9,PinName="InvSize",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_17"
   Begin Object Class=/Script/Engine.MaterialExpressionSceneTexture Name="MaterialExpressionSceneTexture_8"
   End Object
   Begin Object Name="MaterialExpressionSceneTexture_8"
      Coordinates=(Expression=MaterialExpressionSubtract'"MaterialGraphNode_13.MaterialExpressionSubtract_1"')
      SceneTextureId=PPI_CustomDepth
      MaterialExpressionEditorX=-2032
      MaterialExpressionEditorY=656
      MaterialExpressionGuid=52F8C7DD43D02DC47162F3BB4FFA7355
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSceneTexture'"MaterialExpressionSceneTexture_8"'
   NodePosX=-2032
   NodePosY=656
   NodeGuid=FFC75B9E4ACEF0673CAC939DEAF25A74
   CustomProperties Pin (PinId=9839044345A55C546CA1208741682648,PinName="UVs",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_13 D2CF074D4EA63DD5048B2D8017914365,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=981739D244AD9CFB157A93834517A860,PinName="Color",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="rgba",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_19 4839522B4B7E019E7A5C2B89F19C4F3F,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=85D09E034FAF9A93A323C4884B9A7D58,PinName="Size",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=66FD4974447C3ADD3D8B7CA293B1B275,PinName="InvSize",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_18"
   Begin Object Class=/Script/Engine.MaterialExpressionSubtract Name="MaterialExpressionSubtract_2"
   End Object
   Begin Object Name="MaterialExpressionSubtract_2"
      A=(Expression=MaterialExpressionSceneTexture'"MaterialGraphNode_14.MaterialExpressionSceneTexture_3"',Mask=1,MaskR=1,MaskG=1,MaskB=1,MaskA=1)
      B=(Expression=MaterialExpressionSceneTexture'"MaterialGraphNode_15.MaterialExpressionSceneTexture_6"',Mask=1,MaskR=1,MaskG=1,MaskB=1,MaskA=1)
      MaterialExpressionEditorX=-1699
      MaterialExpressionEditorY=339
      MaterialExpressionGuid=FAC86CC0409EA029AA5C238E59278C57
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSubtract'"MaterialExpressionSubtract_2"'
   NodePosX=-1699
   NodePosY=339
   NodeGuid=A3E5210143F46CE791CED7A9D21BA6C3
   CustomProperties Pin (PinId=66D013F44AC2019514616294114E7308,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_14 05090A1E4497156685AD89B66691764C,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=0EAD1630472F82BBB0FE2ABFB7B729A6,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_15 46FD58604FF29C181BB579B66B265E70,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=AD1A8FF548D425E70A3A36BC6B8FBC10,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_20 67B9C9C14E69BF0E81A00C8B910EFC94,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_19"
   Begin Object Class=/Script/Engine.MaterialExpressionSubtract Name="MaterialExpressionSubtract_3"
   End Object
   Begin Object Name="MaterialExpressionSubtract_3"
      A=(Expression=MaterialExpressionSceneTexture'"MaterialGraphNode_16.MaterialExpressionSceneTexture_7"',Mask=1,MaskR=1,MaskG=1,MaskB=1,MaskA=1)
      B=(Expression=MaterialExpressionSceneTexture'"MaterialGraphNode_17.MaterialExpressionSceneTexture_8"',Mask=1,MaskR=1,MaskG=1,MaskB=1,MaskA=1)
      MaterialExpressionEditorX=-1696
      MaterialExpressionEditorY=560
      MaterialExpressionGuid=14EB95F54CAF5F652576E9B06B09D7D2
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSubtract'"MaterialExpressionSubtract_3"'
   NodePosX=-1696
   NodePosY=560
   NodeGuid=38B9C78641DB6F4D6430E3B90BBB9D11
   CustomProperties Pin (PinId=AF143D5D49782637C4998C836280D3FA,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_16 45826F9E408895666B856E9953EB1773,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=4839522B4B7E019E7A5C2B89F19C4F3F,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_17 981739D244AD9CFB157A93834517A860,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=74FE1D4B47340B5AAE5220B7B4E7A756,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_21 F8578A624B8E173129B77CA6B9FC0444,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_20"
   Begin Object Class=/Script/Engine.MaterialExpressionComponentMask Name="MaterialExpressionComponentMask_2"
   End Object
   Begin Object Name="MaterialExpressionComponentMask_2"
      Input=(Expression=MaterialExpressionSubtract'"MaterialGraphNode_18.MaterialExpressionSubtract_2"')
      R=True
      MaterialExpressionEditorX=-1568
      MaterialExpressionEditorY=336
      MaterialExpressionGuid=8F0CA24448DFC0BE95DD539FD9CAE123
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionComponentMask'"MaterialExpressionComponentMask_2"'
   NodePosX=-1568
   NodePosY=336
   NodeGuid=3C27D10C4787E0FC2094788A2E30BE38
   CustomProperties Pin (PinId=67B9C9C14E69BF0E81A00C8B910EFC94,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_18 AD1A8FF548D425E70A3A36BC6B8FBC10,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=31FF5AB440B653EED5871FA5329508C3,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_22 3BD87BBA4EF07D45F662DD9C8CB6B867,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_21"
   Begin Object Class=/Script/Engine.MaterialExpressionComponentMask Name="MaterialExpressionComponentMask_3"
   End Object
   Begin Object Name="MaterialExpressionComponentMask_3"
      Input=(Expression=MaterialExpressionSubtract'"MaterialGraphNode_19.MaterialExpressionSubtract_3"')
      R=True
      MaterialExpressionEditorX=-1568
      MaterialExpressionEditorY=560
      MaterialExpressionGuid=A532C81D49E82520FA13A79F0AB3A0AD
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionComponentMask'"MaterialExpressionComponentMask_3"'
   NodePosX=-1568
   NodePosY=560
   NodeGuid=17B361344EEC0CF4C73084A18266AE2C
   CustomProperties Pin (PinId=F8578A624B8E173129B77CA6B9FC0444,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_19 74FE1D4B47340B5AAE5220B7B4E7A756,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D8F807BB42CC5490D4797386DD92E553,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_24 946431B1460C1A22249D90A08DB56018,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_22"
   Begin Object Class=/Script/Engine.MaterialExpressionDivide Name="MaterialExpressionDivide_0"
   End Object
   Begin Object Name="MaterialExpressionDivide_0"
      A=(Expression=MaterialExpressionComponentMask'"MaterialGraphNode_20.MaterialExpressionComponentMask_2"')
      B=(Expression=MaterialExpressionConstant'"MaterialGraphNode_23.MaterialExpressionConstant_2"')
      MaterialExpressionEditorX=-1376
      MaterialExpressionEditorY=336
      MaterialExpressionGuid=612837FE47645E74542A7D8E0DA57DAC
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionDivide'"MaterialExpressionDivide_0"'
   NodePosX=-1376
   NodePosY=336
   NodeGuid=5A296AC946646E7A30408FB8EB39C590
   CustomProperties Pin (PinId=3BD87BBA4EF07D45F662DD9C8CB6B867,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_20 31FF5AB440B653EED5871FA5329508C3,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=14E53F6A41EFD2DD8EC8F0BE3475977E,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_23 1377DC0B47F36B161E71FA8988E979D2,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=74003B5A4E5410D126E56D8D1A67C608,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_25 ABCB3BA247AEA2206DD97BA1C1E5E913,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_23"
   Begin Object Class=/Script/Engine.MaterialExpressionConstant Name="MaterialExpressionConstant_2"
   End Object
   Begin Object Name="MaterialExpressionConstant_2"
      R=16380.000000
      MaterialExpressionEditorX=-1568
      MaterialExpressionEditorY=464
      MaterialExpressionGuid=95B7BFD94F18C16239FC76A1A00FFE40
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionConstant'"MaterialExpressionConstant_2"'
   NodePosX=-1568
   NodePosY=464
   NodeGuid=D311D9904BC422C1EA0F7A914E62C871
   CustomProperties Pin (PinId=1377DC0B47F36B161E71FA8988E979D2,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_22 14E53F6A41EFD2DD8EC8F0BE3475977E,MaterialGraphNode_24 A80B2A464A271B23FCF47DAF6CE4D2CA,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_24"
   Begin Object Class=/Script/Engine.MaterialExpressionDivide Name="MaterialExpressionDivide_1"
   End Object
   Begin Object Name="MaterialExpressionDivide_1"
      A=(Expression=MaterialExpressionComponentMask'"MaterialGraphNode_21.MaterialExpressionComponentMask_3"')
      B=(Expression=MaterialExpressionConstant'"MaterialGraphNode_23.MaterialExpressionConstant_2"')
      MaterialExpressionEditorX=-1376
      MaterialExpressionEditorY=528
      MaterialExpressionGuid=AAED7D664D5918E3C6A6D6AC601A81BC
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionDivide'"MaterialExpressionDivide_1"'
   NodePosX=-1376
   NodePosY=528
   NodeGuid=64E59DEC49B6AD78F396F09DE01A0B87
   CustomProperties Pin (PinId=946431B1460C1A22249D90A08DB56018,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_21 D8F807BB42CC5490D4797386DD92E553,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=A80B2A464A271B23FCF47DAF6CE4D2CA,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_23 1377DC0B47F36B161E71FA8988E979D2,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=899DDC4A410C5E367AA1C5926B380418,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_26 A61CE9FE46040AFE9CBE8193BC2ADEBB,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_25"
   Begin Object Class=/Script/Engine.MaterialExpressionAbs Name="MaterialExpressionAbs_0"
   End Object
   Begin Object Name="MaterialExpressionAbs_0"
      Input=(Expression=MaterialExpressionDivide'"MaterialGraphNode_22.MaterialExpressionDivide_0"')
      MaterialExpressionEditorX=-1248
      MaterialExpressionEditorY=336
      MaterialExpressionGuid=1A2E21A64E51766E7E978AADB3EEE94C
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAbs'"MaterialExpressionAbs_0"'
   NodePosX=-1248
   NodePosY=336
   NodeGuid=1ACD7E0D4FE36D027C369D8B2B37E170
   CustomProperties Pin (PinId=ABCB3BA247AEA2206DD97BA1C1E5E913,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_22 74003B5A4E5410D126E56D8D1A67C608,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=9C82E5584B9F273F4E1209B28427BAE1,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_27 A4890D6E492800B68DF15A92CC659D9D,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_26"
   Begin Object Class=/Script/Engine.MaterialExpressionAbs Name="MaterialExpressionAbs_1"
   End Object
   Begin Object Name="MaterialExpressionAbs_1"
      Input=(Expression=MaterialExpressionDivide'"MaterialGraphNode_24.MaterialExpressionDivide_1"')
      MaterialExpressionEditorX=-1248
      MaterialExpressionEditorY=528
      MaterialExpressionGuid=364E97AB40F274E73224C0AE5C63B556
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAbs'"MaterialExpressionAbs_1"'
   NodePosX=-1248
   NodePosY=528
   NodeGuid=D3CBD74740732F4C94E2C7918AA51223
   CustomProperties Pin (PinId=A61CE9FE46040AFE9CBE8193BC2ADEBB,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_24 899DDC4A410C5E367AA1C5926B380418,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D83FB4BF4149B1D8F3E8A2AA43B64D71,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_28 2EAB3E8C46855641666548B6FE499733,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_27"
   Begin Object Class=/Script/Engine.MaterialExpressionFloor Name="MaterialExpressionFloor_0"
   End Object
   Begin Object Name="MaterialExpressionFloor_0"
      Input=(Expression=MaterialExpressionAbs'"MaterialGraphNode_25.MaterialExpressionAbs_0"')
      MaterialExpressionEditorX=-1136
      MaterialExpressionEditorY=336
      MaterialExpressionGuid=E76FC4F048BFE757C706ABB412A78152
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionFloor'"MaterialExpressionFloor_0"'
   NodePosX=-1136
   NodePosY=336
   NodeGuid=F4BD2D3C4E199759645E06992CCAAD9B
   CustomProperties Pin (PinId=A4890D6E492800B68DF15A92CC659D9D,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_25 9C82E5584B9F273F4E1209B28427BAE1,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=5326412C4E61AEBFBB150191A9053D46,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_29 30D6110142A4C638BCED00A048804738,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_28"
   Begin Object Class=/Script/Engine.MaterialExpressionFloor Name="MaterialExpressionFloor_1"
   End Object
   Begin Object Name="MaterialExpressionFloor_1"
      Input=(Expression=MaterialExpressionAbs'"MaterialGraphNode_26.MaterialExpressionAbs_1"')
      MaterialExpressionEditorX=-1136
      MaterialExpressionEditorY=528
      MaterialExpressionGuid=A36932F24CC1390CCB68F6814087A401
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionFloor'"MaterialExpressionFloor_1"'
   NodePosX=-1136
   NodePosY=528
   NodeGuid=0535E45E48C5A781EB36F38CCE80A773
   CustomProperties Pin (PinId=2EAB3E8C46855641666548B6FE499733,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_26 D83FB4BF4149B1D8F3E8A2AA43B64D71,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=915DDA634E3F8612D4D95494B012EBE3,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_29 BA8EBD8546301E975306579EF4EA044A,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_29"
   Begin Object Class=/Script/Engine.MaterialExpressionAdd Name="MaterialExpressionAdd_2"
   End Object
   Begin Object Name="MaterialExpressionAdd_2"
      A=(Expression=MaterialExpressionFloor'"MaterialGraphNode_27.MaterialExpressionFloor_0"')
      B=(Expression=MaterialExpressionFloor'"MaterialGraphNode_28.MaterialExpressionFloor_1"')
      MaterialExpressionEditorX=-1040
      MaterialExpressionEditorY=416
      MaterialExpressionGuid=1D39D46F40B86821834D7D852ABA134E
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAdd'"MaterialExpressionAdd_2"'
   NodePosX=-1040
   NodePosY=416
   NodeGuid=91FE377146338E75CF6F0A9785CFFB1B
   CustomProperties Pin (PinId=30D6110142A4C638BCED00A048804738,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_27 5326412C4E61AEBFBB150191A9053D46,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=BA8EBD8546301E975306579EF4EA044A,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_28 915DDA634E3F8612D4D95494B012EBE3,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=B7A04AB942112FAFE08391BE384C0044,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_30 743FF52C447E17F59E25DBBF958E0955,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_30"
   Begin Object Class=/Script/Engine.MaterialExpressionClamp Name="MaterialExpressionClamp_0"
   End Object
   Begin Object Name="MaterialExpressionClamp_0"
      Input=(Expression=MaterialExpressionAdd'"MaterialGraphNode_29.MaterialExpressionAdd_2"')
      MaterialExpressionEditorX=-880
      MaterialExpressionEditorY=400
      MaterialExpressionGuid=1F9D4F804A6B34533E28AEA3D374A902
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionClamp'"MaterialExpressionClamp_0"'
   NodePosX=-880
   NodePosY=400
   NodeGuid=B4018C03432181CC35424FA8368D6280
   CustomProperties Pin (PinId=743FF52C447E17F59E25DBBF958E0955,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_29 B7A04AB942112FAFE08391BE384C0044,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=3A33D8644F218872728A88911F440A03,PinName="Min",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=F4D62D804016701A3301158CA973D214,PinName="Max",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=EE7773FE4F89FC3A5238C386CB238E34,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_34 E5E323E84544C831A58E998D15C45F89,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_31"
   Begin Object Class=/Script/Engine.MaterialExpressionVectorParameter Name="MaterialExpressionVectorParameter_0"
   End Object
   Begin Object Name="MaterialExpressionVectorParameter_0"
      DefaultValue=(R=0.989028,G=0.000000,B=1.000000,A=1.000000)
      ParameterName="EdgeColor"
      ExpressionGUID=82228D00476641593EAFE3BBDC6AB610
      MaterialExpressionEditorX=-1456
      MaterialExpressionEditorY=-128
      MaterialExpressionGuid=E92DB68740B0BF16DA0EB09500B6ECA8
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionVectorParameter'"MaterialExpressionVectorParameter_0"'
   NodePosX=-1456
   NodePosY=-128
   bCanRenameNode=True
   NodeGuid=B562919A4D2F42426E4BA89C76254B2B
   CustomProperties Pin (PinId=B2D944654DC7E174C4C08DA02E573DA9,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_32 F8C3F52B41E1E09471485791B3C25E81,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=383833D34A872A9C20D831A5ACBAD2A0,PinName="Output2",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="red",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=DE15C0664A0E9B1184CB319E58FAE535,PinName="Output3",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="green",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=0DD104714332A9D5BAA152B9AB9F5745,PinName="Output4",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="blue",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=99411DA34B6CD931653459A0D400A9C8,PinName="Output5",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="alpha",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_32 ADEE37A04E540DA95E9C42953A51845F,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_32"
   Begin Object Class=/Script/Engine.MaterialExpressionAppendVector Name="MaterialExpressionAppendVector_4"
   End Object
   Begin Object Name="MaterialExpressionAppendVector_4"
      A=(Expression=MaterialExpressionVectorParameter'"MaterialGraphNode_31.MaterialExpressionVectorParameter_0"',Mask=1,MaskR=1,MaskG=1,MaskB=1)
      B=(Expression=MaterialExpressionVectorParameter'"MaterialGraphNode_31.MaterialExpressionVectorParameter_0"',OutputIndex=4,Mask=1,MaskA=1)
      MaterialExpressionEditorX=-1216
      MaterialExpressionEditorY=-48
      MaterialExpressionGuid=4530D9CC494D4D7F877E5B9165A0564A
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionAppendVector'"MaterialExpressionAppendVector_4"'
   NodePosX=-1216
   NodePosY=-48
   NodeGuid=5319582B4A478490719103A4362EFDBC
   CustomProperties Pin (PinId=F8C3F52B41E1E09471485791B3C25E81,PinName="A",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_31 B2D944654DC7E174C4C08DA02E573DA9,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=ADEE37A04E540DA95E9C42953A51845F,PinName="B",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_31 99411DA34B6CD931653459A0D400A9C8,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=F9AC305444B7B31BF04F86961991C7C7,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 8DDD282B4F80588BFE5E86A9A74283B2,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_33"
   Begin Object Class=/Script/Engine.MaterialExpressionTime Name="MaterialExpressionTime_0"
   End Object
   Begin Object Name="MaterialExpressionTime_0"
      MaterialExpressionEditorX=-2720
      MaterialExpressionEditorY=-16
      MaterialExpressionGuid=DE43325141EDB84E5BC131B6208193AF
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionTime'"MaterialExpressionTime_0"'
   NodePosX=-2720
   NodePosY=-16
   NodeGuid=FBA30DD84939160BED3D15AE4C982124
   CustomProperties Pin (PinId=ACACA9B8467DA7E9B4685888605487CE,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_35 5C512A8E43B6D4C11BE643BFAE17EA0D,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_34"
   Begin Object Class=/Script/Engine.MaterialExpressionMultiply Name="MaterialExpressionMultiply_2"
   End Object
   Begin Object Name="MaterialExpressionMultiply_2"
      A=(Expression=MaterialExpressionLinearInterpolate'"MaterialGraphNode_37.MaterialExpressionLinearInterpolate_2"')
      B=(Expression=MaterialExpressionClamp'"MaterialGraphNode_30.MaterialExpressionClamp_0"')
      MaterialExpressionEditorX=-848
      MaterialExpressionEditorY=224
      MaterialExpressionGuid=DA97CA72429033E59A001BACD1B5E733
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionMultiply'"MaterialExpressionMultiply_2"'
   NodePosX=-848
   NodePosY=224
   NodeGuid=EAD19EB64BA494FB0ED53CB88FCB7D0E
   CustomProperties Pin (PinId=69A1B0874F7E1B1806BEF9811449463A,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_37 3D9158144250FAB2D8F9D9B30D149FC3,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=E5E323E84544C831A58E998D15C45F89,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_30 EE7773FE4F89FC3A5238C386CB238E34,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=06EB87624354CFEA0424488E4A9BFD02,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 C410ED8C467745FE48E45C853A545951,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_35"
   Begin Object Class=/Script/Engine.MaterialExpressionSine Name="MaterialExpressionSine_3"
   End Object
   Begin Object Name="MaterialExpressionSine_3"
      Input=(Expression=MaterialExpressionTime'"MaterialGraphNode_33.MaterialExpressionTime_0"')
      Period=2.000000
      MaterialExpressionEditorX=-2496
      MaterialExpressionGuid=D1DA994C4B762701016A758331BEA001
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSine'"MaterialExpressionSine_3"'
   NodePosX=-2496
   NodeGuid=DA049B9D4679B8BE89503A8F673C3DA9
   CustomProperties Pin (PinId=5C512A8E43B6D4C11BE643BFAE17EA0D,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_33 ACACA9B8467DA7E9B4685888605487CE,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=73F57D974BA07ED0FF78AE8689CD18AB,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_36 6299B65943E2925E1FE99C830B6D73EC,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_36"
   Begin Object Class=/Script/Engine.MaterialExpressionClamp Name="MaterialExpressionClamp_4"
   End Object
   Begin Object Name="MaterialExpressionClamp_4"
      Input=(Expression=MaterialExpressionSine'"MaterialGraphNode_35.MaterialExpressionSine_3"')
      MaterialExpressionEditorX=-2352
      MaterialExpressionGuid=A81F6AEF4A75980FA83FF3A1BBFE7F5F
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionClamp'"MaterialExpressionClamp_4"'
   NodePosX=-2352
   NodeGuid=4318F194473ED05C7254698E85C2820F
   CustomProperties Pin (PinId=6299B65943E2925E1FE99C830B6D73EC,PinName="Input",PinFriendlyName=" ",PinType.PinCategory="required",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_35 73F57D974BA07ED0FF78AE8689CD18AB,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=5BA8198D4FA41101C771C0AAA13A85B6,PinName="Min",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=CE48248C442C7B71B8A8E09F2A8536FE,PinName="Max",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=D1CAE573467EFA7273F5FCAE0B871DBF,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_37 ABFE650D40BF306841ADDEBFBD112969,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_37"
   Begin Object Class=/Script/Engine.MaterialExpressionLinearInterpolate Name="MaterialExpressionLinearInterpolate_2"
   End Object
   Begin Object Name="MaterialExpressionLinearInterpolate_2"
      Alpha=(Expression=MaterialExpressionClamp'"MaterialGraphNode_36.MaterialExpressionClamp_4"')
      ConstA=1.000000
      ConstB=0.050000
      MaterialExpressionEditorX=-2000
      MaterialExpressionEditorY=-16
      MaterialExpressionGuid=46EB14DD40CAE034F6BA95BDA2C426C0
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionLinearInterpolate'"MaterialExpressionLinearInterpolate_2"'
   NodePosX=-2000
   NodePosY=-16
   NodeGuid=B48BFBFA4345BEE7816A87A7AE7467AC
   CustomProperties Pin (PinId=FDD06D2F46D7F2265E39B6B150ECD02A,PinName="A",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=9C6709954D1DA98FF98C199C553B78AE,PinName="B",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=ABFE650D40BF306841ADDEBFBD112969,PinName="Alpha",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_36 D1CAE573467EFA7273F5FCAE0B871DBF,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=3D9158144250FAB2D8F9D9B30D149FC3,PinName="Output",PinFriendlyName=" ",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_34 69A1B0874F7E1B1806BEF9811449463A,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object
Begin Object Class=/Script/UnrealEd.MaterialGraphNode Name="MaterialGraphNode_38"
   Begin Object Class=/Script/Engine.MaterialExpressionSceneTexture Name="MaterialExpressionSceneTexture_0"
   End Object
   Begin Object Name="MaterialExpressionSceneTexture_0"
      SceneTextureId=PPI_PostProcessInput0
      MaterialExpressionEditorX=-1040
      MaterialExpressionEditorY=-176
      MaterialExpressionGuid=E981DE424880DB00AAA5AEB5A9FBA5C5
      Material=PreviewMaterial'"/Engine/Transient.PreviewMaterial_1"'
   End Object
   MaterialExpression=MaterialExpressionSceneTexture'"MaterialExpressionSceneTexture_0"'
   NodePosX=-1040
   NodePosY=-176
   NodeGuid=3656EE79467E1427294633AD2549B375
   CustomProperties Pin (PinId=E3B186234ED546DAAF3E4EAA5BD86DB4,PinName="UVs",PinType.PinCategory="optional",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=5ADD66E44050C33664C4A5986B2382A4,PinName="Color",Direction="EGPD_Output",PinType.PinCategory="mask",PinType.PinSubCategory="rgba",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,LinkedTo=(MaterialGraphNode_0 3EF0ADDF427C6243CF105D9BEC7098F1,),PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=F208FE09434148C6D647049E7ECB0A2B,PinName="Size",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
   CustomProperties Pin (PinId=7174854F4B84BBBE9653A0AF99BC3AE3,PinName="InvSize",Direction="EGPD_Output",PinType.PinCategory="",PinType.PinSubCategory="",PinType.PinSubCategoryObject=None,PinType.PinSubCategoryMemberReference=(),PinType.PinValueType=(),PinType.ContainerType=None,PinType.bIsArray=False,PinType.bIsReference=False,PinType.bIsConst=False,PinType.bIsWeakPointer=False,PersistentGuid=00000000000000000000000000000000,bHidden=False,bNotConnectable=False,bDefaultValueIsReadOnly=False,bDefaultValueIsIgnored=False,bAdvancedView=False,bOrphanedPin=False,)
End Object

{% endcodeblock %}

![参数设置](02.jpg)
![添加后期](03.jpg)
![设置物体](04.jpg)