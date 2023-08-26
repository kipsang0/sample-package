# SwaggerClient-php
CloudPap Console API

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: v1
- Build package: io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com//.git"
    }
  ],
  "require": {
    "/": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: Basic
$config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setUsername('YOUR_USERNAME')
    ->setPassword('YOUR_PASSWORD');

$apiInstance = new Swagger\Client\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$data = new \Swagger\Client\Model\BillingCard(); // \Swagger\Client\Model\BillingCard | 

try {
    $result = $apiInstance->billingCardsCreate($data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->billingCardsCreate: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost:8000/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BillingApi* | [**billingCardsCreate**](docs/Api/BillingApi.md#billingcardscreate) | **POST** /billing/cards/ | 
*BillingApi* | [**billingCardsDefault**](docs/Api/BillingApi.md#billingcardsdefault) | **PATCH** /billing/cards/{id}/default/ | 
*BillingApi* | [**billingCardsDelete**](docs/Api/BillingApi.md#billingcardsdelete) | **DELETE** /billing/cards/{id}/ | 
*BillingApi* | [**billingCardsList**](docs/Api/BillingApi.md#billingcardslist) | **GET** /billing/cards/ | 
*BillingApi* | [**billingCardsRead**](docs/Api/BillingApi.md#billingcardsread) | **GET** /billing/cards/{id}/ | 
*BillingApi* | [**billingCustomersAppliedCoupons**](docs/Api/BillingApi.md#billingcustomersappliedcoupons) | **GET** /billing/customers/{id}/applied-coupons/ | 
*BillingApi* | [**billingCustomersApplyCoupon**](docs/Api/BillingApi.md#billingcustomersapplycoupon) | **POST** /billing/customers/{id}/apply-coupon/ | 
*BillingApi* | [**billingCustomersBillingWallet**](docs/Api/BillingApi.md#billingcustomersbillingwallet) | **GET** /billing/customers/{id}/billing-wallet/ | 
*BillingApi* | [**billingCustomersList**](docs/Api/BillingApi.md#billingcustomerslist) | **GET** /billing/customers/ | 
*BillingApi* | [**billingCustomersPartialUpdate**](docs/Api/BillingApi.md#billingcustomerspartialupdate) | **PATCH** /billing/customers/{id}/ | 
*BillingApi* | [**billingCustomersRead**](docs/Api/BillingApi.md#billingcustomersread) | **GET** /billing/customers/{id}/ | 
*BillingApi* | [**billingCustomersUpdate**](docs/Api/BillingApi.md#billingcustomersupdate) | **PUT** /billing/customers/{id}/ | 
*BillingApi* | [**billingInvoicesList**](docs/Api/BillingApi.md#billinginvoiceslist) | **GET** /billing/invoices/ | 
*BillingApi* | [**billingInvoicesRead**](docs/Api/BillingApi.md#billinginvoicesread) | **GET** /billing/invoices/{id}/ | 
*BillingApi* | [**billingPaymentMethodsCreate**](docs/Api/BillingApi.md#billingpaymentmethodscreate) | **POST** /billing/payment-methods/ | 
*BillingApi* | [**billingPaymentMethodsDelete**](docs/Api/BillingApi.md#billingpaymentmethodsdelete) | **DELETE** /billing/payment-methods/{id}/ | 
*BillingApi* | [**billingPaymentMethodsList**](docs/Api/BillingApi.md#billingpaymentmethodslist) | **GET** /billing/payment-methods/ | 
*BillingApi* | [**billingPaymentMethodsPartialUpdate**](docs/Api/BillingApi.md#billingpaymentmethodspartialupdate) | **PATCH** /billing/payment-methods/{id}/ | 
*BillingApi* | [**billingPaymentMethodsRead**](docs/Api/BillingApi.md#billingpaymentmethodsread) | **GET** /billing/payment-methods/{id}/ | 
*BillingApi* | [**billingPaymentMethodsUpdate**](docs/Api/BillingApi.md#billingpaymentmethodsupdate) | **PUT** /billing/payment-methods/{id}/ | 
*BillingApi* | [**billingTransactionsList**](docs/Api/BillingApi.md#billingtransactionslist) | **GET** /billing/transactions/ | 
*BillingApi* | [**billingTransactionsRead**](docs/Api/BillingApi.md#billingtransactionsread) | **GET** /billing/transactions/{id}/ | 
*KubeAppsApi* | [**kubeAppsList**](docs/Api/KubeAppsApi.md#kubeappslist) | **GET** /kube-apps/ | 
*KubeAppsApi* | [**kubeAppsRead**](docs/Api/KubeAppsApi.md#kubeappsread) | **GET** /kube-apps/{id}/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesConnectDomain**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstancesconnectdomain) | **POST** /kube-apps-instances/{id}/connect-domain/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesCreate**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstancescreate) | **POST** /kube-apps-instances/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesDelete**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstancesdelete) | **DELETE** /kube-apps-instances/{id}/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesList**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstanceslist) | **GET** /kube-apps-instances/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesPartialUpdate**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstancespartialupdate) | **PATCH** /kube-apps-instances/{id}/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesRead**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstancesread) | **GET** /kube-apps-instances/{id}/ | 
*KubeAppsInstancesApi* | [**kubeAppsInstancesUpdate**](docs/Api/KubeAppsInstancesApi.md#kubeappsinstancesupdate) | **PUT** /kube-apps-instances/{id}/ | 
*KubeAppsLocationsApi* | [**kubeAppsLocationsList**](docs/Api/KubeAppsLocationsApi.md#kubeappslocationslist) | **GET** /kube-apps-locations/ | 
*KubeAppsLocationsApi* | [**kubeAppsLocationsRead**](docs/Api/KubeAppsLocationsApi.md#kubeappslocationsread) | **GET** /kube-apps-locations/{id}/ | 
*KubeAppsTemplatesApi* | [**kubeAppsTemplatesList**](docs/Api/KubeAppsTemplatesApi.md#kubeappstemplateslist) | **GET** /kube-apps-templates/ | 
*KubeAppsTemplatesApi* | [**kubeAppsTemplatesRead**](docs/Api/KubeAppsTemplatesApi.md#kubeappstemplatesread) | **GET** /kube-apps-templates/{id}/ | 
*KubeAppsVersionsApi* | [**kubeAppsVersionsList**](docs/Api/KubeAppsVersionsApi.md#kubeappsversionslist) | **GET** /kube-apps-versions/ | 
*KubeAppsVersionsApi* | [**kubeAppsVersionsRead**](docs/Api/KubeAppsVersionsApi.md#kubeappsversionsread) | **GET** /kube-apps-versions/{id}/ | 
*MarketingApi* | [**marketingFocusItemsList**](docs/Api/MarketingApi.md#marketingfocusitemslist) | **GET** /marketing/focus-items/ | 
*MarketingApi* | [**marketingFocusItemsRead**](docs/Api/MarketingApi.md#marketingfocusitemsread) | **GET** /marketing/focus-items/{id}/ | 
*SocialAuthApi* | [**socialAuthCreate**](docs/Api/SocialAuthApi.md#socialauthcreate) | **POST** /social-auth/ | 
*SocialAuthApi* | [**socialAuthGithubAuth**](docs/Api/SocialAuthApi.md#socialauthgithubauth) | **POST** /social-auth/github/ | 
*SocialAuthApi* | [**socialAuthGoogleAuth**](docs/Api/SocialAuthApi.md#socialauthgoogleauth) | **POST** /social-auth/google/ | 
*TokenApi* | [**tokenVerifyCreate**](docs/Api/TokenApi.md#tokenverifycreate) | **POST** /token/verify/ | 
*VirtualMachineBackupTemplatesApi* | [**virtualMachineBackupTemplatesList**](docs/Api/VirtualMachineBackupTemplatesApi.md#virtualmachinebackuptemplateslist) | **GET** /virtual-machine-backup-templates/ | 
*VirtualMachineBackupTemplatesApi* | [**virtualMachineBackupTemplatesRead**](docs/Api/VirtualMachineBackupTemplatesApi.md#virtualmachinebackuptemplatesread) | **GET** /virtual-machine-backup-templates/{id}/ | 
*VirtualMachineBackupsApi* | [**virtualMachineBackupsDelete**](docs/Api/VirtualMachineBackupsApi.md#virtualmachinebackupsdelete) | **DELETE** /virtual-machine-backups/{id}/ | 
*VirtualMachineBackupsApi* | [**virtualMachineBackupsList**](docs/Api/VirtualMachineBackupsApi.md#virtualmachinebackupslist) | **GET** /virtual-machine-backups/ | 
*VirtualMachineBackupsApi* | [**virtualMachineBackupsRead**](docs/Api/VirtualMachineBackupsApi.md#virtualmachinebackupsread) | **GET** /virtual-machine-backups/{id}/ | 
*VirtualMachineBackupsApi* | [**virtualMachineBackupsRestore**](docs/Api/VirtualMachineBackupsApi.md#virtualmachinebackupsrestore) | **POST** /virtual-machine-backups/{id}/restore/ | 
*VirtualMachineImagesApi* | [**virtualMachineImagesList**](docs/Api/VirtualMachineImagesApi.md#virtualmachineimageslist) | **GET** /virtual-machine-images/ | 
*VirtualMachineImagesApi* | [**virtualMachineImagesRead**](docs/Api/VirtualMachineImagesApi.md#virtualmachineimagesread) | **GET** /virtual-machine-images/{id}/ | 
*VirtualMachineLocationsApi* | [**virtualMachineLocationsList**](docs/Api/VirtualMachineLocationsApi.md#virtualmachinelocationslist) | **GET** /virtual-machine-locations/ | 
*VirtualMachineLocationsApi* | [**virtualMachineLocationsRead**](docs/Api/VirtualMachineLocationsApi.md#virtualmachinelocationsread) | **GET** /virtual-machine-locations/{id}/ | 
*VirtualMachineTemplatesApi* | [**virtualMachineTemplatesList**](docs/Api/VirtualMachineTemplatesApi.md#virtualmachinetemplateslist) | **GET** /virtual-machine-templates/ | 
*VirtualMachineTemplatesApi* | [**virtualMachineTemplatesRead**](docs/Api/VirtualMachineTemplatesApi.md#virtualmachinetemplatesread) | **GET** /virtual-machine-templates/{id}/ | 
*VirtualMachinesApi* | [**virtualMachinesChangeVmBackupTemplate**](docs/Api/VirtualMachinesApi.md#virtualmachineschangevmbackuptemplate) | **POST** /virtual-machines/{id}/change-backup-template/ | 
*VirtualMachinesApi* | [**virtualMachinesChangeVmTemplate**](docs/Api/VirtualMachinesApi.md#virtualmachineschangevmtemplate) | **POST** /virtual-machines/{id}/change-template/ | 
*VirtualMachinesApi* | [**virtualMachinesCreate**](docs/Api/VirtualMachinesApi.md#virtualmachinescreate) | **POST** /virtual-machines/ | 
*VirtualMachinesApi* | [**virtualMachinesDelete**](docs/Api/VirtualMachinesApi.md#virtualmachinesdelete) | **DELETE** /virtual-machines/{id}/ | 
*VirtualMachinesApi* | [**virtualMachinesDisableVmBackup**](docs/Api/VirtualMachinesApi.md#virtualmachinesdisablevmbackup) | **POST** /virtual-machines/{id}/disable-backup/ | 
*VirtualMachinesApi* | [**virtualMachinesList**](docs/Api/VirtualMachinesApi.md#virtualmachineslist) | **GET** /virtual-machines/ | 
*VirtualMachinesApi* | [**virtualMachinesPartialUpdate**](docs/Api/VirtualMachinesApi.md#virtualmachinespartialupdate) | **PATCH** /virtual-machines/{id}/ | 
*VirtualMachinesApi* | [**virtualMachinesPauseVm**](docs/Api/VirtualMachinesApi.md#virtualmachinespausevm) | **POST** /virtual-machines/{id}/pause/ | 
*VirtualMachinesApi* | [**virtualMachinesRead**](docs/Api/VirtualMachinesApi.md#virtualmachinesread) | **GET** /virtual-machines/{id}/ | 
*VirtualMachinesApi* | [**virtualMachinesRebuildVm**](docs/Api/VirtualMachinesApi.md#virtualmachinesrebuildvm) | **POST** /virtual-machines/{id}/rebuild/ | 
*VirtualMachinesApi* | [**virtualMachinesRestartVm**](docs/Api/VirtualMachinesApi.md#virtualmachinesrestartvm) | **POST** /virtual-machines/{id}/restart/ | 
*VirtualMachinesApi* | [**virtualMachinesSoftRebootVm**](docs/Api/VirtualMachinesApi.md#virtualmachinessoftrebootvm) | **POST** /virtual-machines/{id}/soft-reboot/ | 
*VirtualMachinesApi* | [**virtualMachinesStartVm**](docs/Api/VirtualMachinesApi.md#virtualmachinesstartvm) | **POST** /virtual-machines/{id}/start/ | 
*VirtualMachinesApi* | [**virtualMachinesStopVm**](docs/Api/VirtualMachinesApi.md#virtualmachinesstopvm) | **POST** /virtual-machines/{id}/stop/ | 
*VirtualMachinesApi* | [**virtualMachinesTakeVmBackup**](docs/Api/VirtualMachinesApi.md#virtualmachinestakevmbackup) | **POST** /virtual-machines/{id}/take-backup/ | 
*VirtualMachinesApi* | [**virtualMachinesTakeVmSnapshot**](docs/Api/VirtualMachinesApi.md#virtualmachinestakevmsnapshot) | **POST** /virtual-machines/{id}/take-snapshot/ | 
*VirtualMachinesApi* | [**virtualMachinesUnpauseVm**](docs/Api/VirtualMachinesApi.md#virtualmachinesunpausevm) | **POST** /virtual-machines/{id}/unpause/ | 
*VirtualMachinesApi* | [**virtualMachinesUpdate**](docs/Api/VirtualMachinesApi.md#virtualmachinesupdate) | **PUT** /virtual-machines/{id}/ | 


## Documentation For Models

 - [BillingCard](docs/Model/BillingCard.md)
 - [BillingCustomer](docs/Model/BillingCustomer.md)
 - [BillingInvoice](docs/Model/BillingInvoice.md)
 - [BillingPaymentMethod](docs/Model/BillingPaymentMethod.md)
 - [BillingTransaction](docs/Model/BillingTransaction.md)
 - [ConnectDomain](docs/Model/ConnectDomain.md)
 - [CouponClaim](docs/Model/CouponClaim.md)
 - [DocumentEntry](docs/Model/DocumentEntry.md)
 - [KubeApp](docs/Model/KubeApp.md)
 - [KubeAppInstance](docs/Model/KubeAppInstance.md)
 - [KubeAppTemplate](docs/Model/KubeAppTemplate.md)
 - [KubeAppVersion](docs/Model/KubeAppVersion.md)
 - [KubeAppsLocation](docs/Model/KubeAppsLocation.md)
 - [MauticFocusItem](docs/Model/MauticFocusItem.md)
 - [SocialLogin](docs/Model/SocialLogin.md)
 - [TokenVerify](docs/Model/TokenVerify.md)
 - [VirtualMachine](docs/Model/VirtualMachine.md)
 - [VirtualMachineActions](docs/Model/VirtualMachineActions.md)
 - [VirtualMachineBackup](docs/Model/VirtualMachineBackup.md)
 - [VirtualMachineBackupTemplate](docs/Model/VirtualMachineBackupTemplate.md)
 - [VirtualMachineChangeBackupTemplate](docs/Model/VirtualMachineChangeBackupTemplate.md)
 - [VirtualMachineChangeTemplate](docs/Model/VirtualMachineChangeTemplate.md)
 - [VirtualMachineImage](docs/Model/VirtualMachineImage.md)
 - [VirtualMachineLocation](docs/Model/VirtualMachineLocation.md)
 - [VirtualMachineTemplate](docs/Model/VirtualMachineTemplate.md)


## Documentation For Authorization


## Basic

- **Type**: HTTP basic authentication


## Author

info@cloudpap.com

