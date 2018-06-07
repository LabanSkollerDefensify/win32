---
Description: Each of the following sections discusses a function exported by Xenroll.dll. Each section also discusses how to use CertEnroll.dll to replace the function or indicates that no mapping between the two libraries exists.
ms.assetid: 06d8dd6f-7a8d-4da5-a99d-9c9d8fb90cfa
title: Helper Functions
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Helper Functions

Each of the following sections discusses a function exported by Xenroll.dll. Each section also discusses how to use CertEnroll.dll to replace the function or indicates that no mapping between the two libraries exists.

## binaryBlobToString

The [**binaryBlobToString**](https://msdn.microsoft.com/library/windows/desktop/aa385524) function in Xenroll.dll converts a byte array to a string.

Using CertEnroll.dll, you can call the [**VariantByteArrayToString**](/windows/desktop/api/CertEnroll/nf-certenroll-ibinaryconverter-variantbytearraytostring) method on the [**IBinaryConverter**](/windows/desktop/api/CertEnroll/nn-certenroll-ibinaryconverter) interface.

## stringToBinaryBlob

The [**stringToBinaryBlob**](https://msdn.microsoft.com/library/windows/desktop/aa386145) function in Xenroll.dll converts a string to a byte array.

Using CertEnroll.dll, you can call the [**StringToVariantByteArray**](/windows/desktop/api/CertEnroll/nf-certenroll-ibinaryconverter-stringtovariantbytearray) method on the [**IBinaryConverter**](/windows/desktop/api/CertEnroll/nn-certenroll-ibinaryconverter) interface.

## Related topics

<dl> <dt>

[Mapping Xenroll.dll to CertEnroll.dll](mapping-xenroll-dll-to-certenroll-dll.md)
</dt> <dt>

[**IBinaryConverter**](/windows/desktop/api/CertEnroll/nn-certenroll-ibinaryconverter)
</dt> </dl>

 

 


