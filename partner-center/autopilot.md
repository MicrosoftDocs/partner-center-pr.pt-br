---
title: Customize a device's out-of-box experience with Windows Autopilot profiles | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to customize or pre-configure a new device's out-of-box experience with Autopilot profiles before you deliver the device to the customer.
author: maggiepuccievans
ms.author: evansma
keywords: autopilot, windows autopilot, microsoft autopilot, zero-touch deployment, oobe, login screens, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: a07c18fda7de0aa5854fb46a91bea692c033d51c
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253326"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="11ca9-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span><span class="sxs-lookup"><span data-stu-id="11ca9-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="11ca9-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="11ca9-105">**Applies to**</span></span>

- <span data-ttu-id="11ca9-106">CSP direct-bill partners, indirect providers, and indirect resellers</span><span class="sxs-lookup"><span data-stu-id="11ca9-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="11ca9-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span><span class="sxs-lookup"><span data-stu-id="11ca9-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="11ca9-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span><span class="sxs-lookup"><span data-stu-id="11ca9-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="11ca9-109">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)** .</span><span class="sxs-lookup"><span data-stu-id="11ca9-109">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="11ca9-110">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span><span class="sxs-lookup"><span data-stu-id="11ca9-110">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="11ca9-111">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11ca9-111">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="11ca9-112">If you're not already familiar with Autopilot, review the information in these articles:</span><span class="sxs-lookup"><span data-stu-id="11ca9-112">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="11ca9-113">Visão geral do Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="11ca9-113">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="11ca9-114">Autopilot deployment reference guide</span><span class="sxs-lookup"><span data-stu-id="11ca9-114">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="11ca9-115">Visão geral</span><span class="sxs-lookup"><span data-stu-id="11ca9-115">Overview</span></span>

<span data-ttu-id="11ca9-116">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span><span class="sxs-lookup"><span data-stu-id="11ca9-116">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="11ca9-117">The following profile settings were available at the time this article was published:</span><span class="sxs-lookup"><span data-stu-id="11ca9-117">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="11ca9-118">Skip privacy settings.</span><span class="sxs-lookup"><span data-stu-id="11ca9-118">Skip privacy settings.</span></span> <span data-ttu-id="11ca9-119">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span><span class="sxs-lookup"><span data-stu-id="11ca9-119">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="11ca9-120">Disable local admin account creation on the device.</span><span class="sxs-lookup"><span data-stu-id="11ca9-120">Disable local admin account creation on the device.</span></span> <span data-ttu-id="11ca9-121">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span><span class="sxs-lookup"><span data-stu-id="11ca9-121">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="11ca9-122">Automatically set up device for work or school.</span><span class="sxs-lookup"><span data-stu-id="11ca9-122">Automatically set up device for work or school.</span></span> <span data-ttu-id="11ca9-123">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span><span class="sxs-lookup"><span data-stu-id="11ca9-123">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="11ca9-124">Skip Cortana, OneDrive, and OEM registration setup pages.</span><span class="sxs-lookup"><span data-stu-id="11ca9-124">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="11ca9-125">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span><span class="sxs-lookup"><span data-stu-id="11ca9-125">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="11ca9-126">Skip End User License Agreement (EULA).</span><span class="sxs-lookup"><span data-stu-id="11ca9-126">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="11ca9-127">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span><span class="sxs-lookup"><span data-stu-id="11ca9-127">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="11ca9-128">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span><span class="sxs-lookup"><span data-stu-id="11ca9-128">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="11ca9-129">The following profile and device management permissions and limitations apply:</span><span class="sxs-lookup"><span data-stu-id="11ca9-129">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="11ca9-130">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span><span class="sxs-lookup"><span data-stu-id="11ca9-130">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="11ca9-131">You can manage existing devices for your customers that you have added.</span><span class="sxs-lookup"><span data-stu-id="11ca9-131">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="11ca9-132">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span><span class="sxs-lookup"><span data-stu-id="11ca9-132">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="11ca9-133">Create and manage Autopilot profiles in Partner Center</span><span class="sxs-lookup"><span data-stu-id="11ca9-133">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="11ca9-134">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span><span class="sxs-lookup"><span data-stu-id="11ca9-134">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="11ca9-135">Only admin agents can create and apply profiles.</span><span class="sxs-lookup"><span data-stu-id="11ca9-135">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="11ca9-136">Create a new Autopilot profile</span><span class="sxs-lookup"><span data-stu-id="11ca9-136">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="11ca9-137">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span><span class="sxs-lookup"><span data-stu-id="11ca9-137">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="11ca9-138">On the customer's detail page, select **Devices**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-138">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="11ca9-139">Under **Windows Autopilot profiles** select **Add new profile**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-139">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="11ca9-140">Enter the profile's name and description and then configure the OOBE settings.</span><span class="sxs-lookup"><span data-stu-id="11ca9-140">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="11ca9-141">Choose from:</span><span class="sxs-lookup"><span data-stu-id="11ca9-141">Choose from:</span></span>  

   - <span data-ttu-id="11ca9-142">Skip privacy settings in setup</span><span class="sxs-lookup"><span data-stu-id="11ca9-142">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="11ca9-143">Desabilitar a conta de administrador local na instalação</span><span class="sxs-lookup"><span data-stu-id="11ca9-143">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="11ca9-144">Ignorar automaticamente as páginas na instalação</span><span class="sxs-lookup"><span data-stu-id="11ca9-144">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="11ca9-145">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span><span class="sxs-lookup"><span data-stu-id="11ca9-145">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="11ca9-146">Skip end user license agreement (EULA)</span><span class="sxs-lookup"><span data-stu-id="11ca9-146">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="11ca9-147">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span><span class="sxs-lookup"><span data-stu-id="11ca9-147">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="11ca9-148">Selecione **Enviar** quando terminado.</span><span class="sxs-lookup"><span data-stu-id="11ca9-148">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="11ca9-149">Apply an Autopilot profile to customer devices</span><span class="sxs-lookup"><span data-stu-id="11ca9-149">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="11ca9-150">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span><span class="sxs-lookup"><span data-stu-id="11ca9-150">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="11ca9-151">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span><span class="sxs-lookup"><span data-stu-id="11ca9-151">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="11ca9-152">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span><span class="sxs-lookup"><span data-stu-id="11ca9-152">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="11ca9-153">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span><span class="sxs-lookup"><span data-stu-id="11ca9-153">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="11ca9-154">On the customer's detail page, select **Devices**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-154">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="11ca9-155">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-155">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="11ca9-156">The profile you just applied appears in the **Profile** column.</span><span class="sxs-lookup"><span data-stu-id="11ca9-156">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="11ca9-157">Follow the steps below to verify that the profile will be applied successfully to the device.</span><span class="sxs-lookup"><span data-stu-id="11ca9-157">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="11ca9-158">a.</span><span class="sxs-lookup"><span data-stu-id="11ca9-158">a.</span></span>  <span data-ttu-id="11ca9-159">Connect a device to the network and turn it on.</span><span class="sxs-lookup"><span data-stu-id="11ca9-159">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="11ca9-160">b.</span><span class="sxs-lookup"><span data-stu-id="11ca9-160">b.</span></span>  <span data-ttu-id="11ca9-161">Verifique se aparecem as telas OOBE apropriadas (se existirem).</span><span class="sxs-lookup"><span data-stu-id="11ca9-161">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="11ca9-162">c.</span><span class="sxs-lookup"><span data-stu-id="11ca9-162">c.</span></span>  <span data-ttu-id="11ca9-163">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span><span class="sxs-lookup"><span data-stu-id="11ca9-163">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="11ca9-164">Remove an Autopilot profile from a customer's device</span><span class="sxs-lookup"><span data-stu-id="11ca9-164">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="11ca9-165">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span><span class="sxs-lookup"><span data-stu-id="11ca9-165">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="11ca9-166">On the customer's detail page, select **Devices**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-166">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="11ca9-167">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-167">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="11ca9-168">Removing a profile from a device does not delete the profile from your list.</span><span class="sxs-lookup"><span data-stu-id="11ca9-168">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="11ca9-169">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="11ca9-169">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="11ca9-170">Update or delete an Autopilot profile</span><span class="sxs-lookup"><span data-stu-id="11ca9-170">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="11ca9-171">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11ca9-171">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="11ca9-172">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span><span class="sxs-lookup"><span data-stu-id="11ca9-172">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="11ca9-173">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span><span class="sxs-lookup"><span data-stu-id="11ca9-173">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="11ca9-174">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span><span class="sxs-lookup"><span data-stu-id="11ca9-174">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="11ca9-175">On the customer's detail page, select **Devices**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-175">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="11ca9-176">Under **Windows Autopilot profiles** select the profile you need to update.</span><span class="sxs-lookup"><span data-stu-id="11ca9-176">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="11ca9-177">Make the required changes and then select **Submit**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-177">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="11ca9-178">To delete this profile, select **Delete profile** from the upper right corner of the page.</span><span class="sxs-lookup"><span data-stu-id="11ca9-178">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="11ca9-179">Add devices to a customer's account</span><span class="sxs-lookup"><span data-stu-id="11ca9-179">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="11ca9-180">Sales agents and admin agents can add devices to a customer's account.</span><span class="sxs-lookup"><span data-stu-id="11ca9-180">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="11ca9-181">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span><span class="sxs-lookup"><span data-stu-id="11ca9-181">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="11ca9-182">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span><span class="sxs-lookup"><span data-stu-id="11ca9-182">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="11ca9-183">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span><span class="sxs-lookup"><span data-stu-id="11ca9-183">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="11ca9-184">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span><span class="sxs-lookup"><span data-stu-id="11ca9-184">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="11ca9-185">Follow the instructions below to add devices to a customer's account in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11ca9-185">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="11ca9-186">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span><span class="sxs-lookup"><span data-stu-id="11ca9-186">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="11ca9-187">On the customer's detail page, select **Devices**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-187">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="11ca9-188">Under **Apply profiles to devices** select **Add devices**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-188">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="11ca9-189">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11ca9-189">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="11ca9-190">You should have received this .csv file with your device purchase.</span><span class="sxs-lookup"><span data-stu-id="11ca9-190">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="11ca9-191">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="11ca9-191">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="11ca9-192">Upload the .csv file and then select **Save**.</span><span class="sxs-lookup"><span data-stu-id="11ca9-192">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="11ca9-193">If you get an error message while trying to upload the .csv file, check the format of the file.</span><span class="sxs-lookup"><span data-stu-id="11ca9-193">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="11ca9-194">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span><span class="sxs-lookup"><span data-stu-id="11ca9-194">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="11ca9-195">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span><span class="sxs-lookup"><span data-stu-id="11ca9-195">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="11ca9-196">Your .csv file should look something like this:</span><span class="sxs-lookup"><span data-stu-id="11ca9-196">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="11ca9-197">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span><span class="sxs-lookup"><span data-stu-id="11ca9-197">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="11ca9-198">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="11ca9-198">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

<span data-ttu-id="11ca9-199">Note that "Manufacturer name" and "Device model" are case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="11ca9-199">Note that "Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="11ca9-200">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span><span class="sxs-lookup"><span data-stu-id="11ca9-200">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="11ca9-201">Windows Autopilot EULA dismissal</span><span class="sxs-lookup"><span data-stu-id="11ca9-201">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="11ca9-202">IMPORTANT INFORMATION</span><span class="sxs-lookup"><span data-stu-id="11ca9-202">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="11ca9-203">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span><span class="sxs-lookup"><span data-stu-id="11ca9-203">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="11ca9-204">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span><span class="sxs-lookup"><span data-stu-id="11ca9-204">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="11ca9-205">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span><span class="sxs-lookup"><span data-stu-id="11ca9-205">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="11ca9-206">Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta.</span><span class="sxs-lookup"><span data-stu-id="11ca9-206">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="11ca9-207">Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.</span><span class="sxs-lookup"><span data-stu-id="11ca9-207">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
