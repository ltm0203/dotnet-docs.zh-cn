---
title: 类型&lt;typename&gt;不符合 CLS
ms.date: 07/20/2015
f1_keywords:
- bc40041
- vbc40041
helpviewer_keywords:
- BC40041
ms.assetid: 634132c2-5646-44aa-98c6-f773e2e63882
ms.openlocfilehash: 9911b4fe7b88996f17cb5e9eec7d4a5f2c254b76
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33594603"
---
# <a name="type-lttypenamegt-is-not-cls-compliant"></a>类型&lt;typename&gt;不符合 CLS
变量、 属性或函数返回声明具有不符合 CLS 的数据类型。  
  
 应用程序，以符合[语言独立性和独立于语言的组件](../../../standard/language-independence-and-language-independent-components.md)(CLS)，它必须只使用符合 cls 的类型。  
  
 下面的 Visual Basic 数据类型不符合 cls 的：  
  
-   [SByte 数据类型](../../../visual-basic/language-reference/data-types/sbyte-data-type.md)  
  
-   [UInteger 数据类型](../../../visual-basic/language-reference/data-types/uinteger-data-type.md)  
  
-   [ULong 数据类型](../../../visual-basic/language-reference/data-types/ulong-data-type.md)  
  
-   [UShort 数据类型](../../../visual-basic/language-reference/data-types/ushort-data-type.md)  
  
 **错误 ID:** BC40041  
  
## <a name="to-correct-this-error"></a>更正此错误  
  
-   如果你的应用程序需要符合 cls 的将此元素的数据类型更改为最接近的符合 cls 的类型。 例如，如果不需要 2147483647 以上的数值范围，可以使用 `UInteger` 取代 `Integer` 。 如果确实需要更大范围，可以用 `UInteger` 代替 `Long`。  
  
-   如果你的应用程序并不需要符合 cls 的你不需要更改任何内容。 你应注意它是不符合，但是。