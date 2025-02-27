---
slug: /AirdropERC1155
title: AirdropERC1155
hide_title: true
displayed_sidebar: contracts
---

# AirdropERC1155

## Methods

### DEFAULT_ADMIN_ROLE

```solidity
function DEFAULT_ADMIN_ROLE() external view returns (bytes32)
```

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | bytes32 | undefined   |

### addAirdropRecipients

```solidity
function addAirdropRecipients(IAirdropERC1155.AirdropContent[] _contents) external nonpayable
```

#### Parameters

| Name       | Type                             | Description |
| ---------- | -------------------------------- | ----------- |
| \_contents | IAirdropERC1155.AirdropContent[] | undefined   |

### airdrop

```solidity
function airdrop(address _tokenAddress, address _tokenOwner, IAirdropERC1155.AirdropContent[] _contents) external nonpayable
```

#### Parameters

| Name           | Type                             | Description |
| -------------- | -------------------------------- | ----------- |
| \_tokenAddress | address                          | undefined   |
| \_tokenOwner   | address                          | undefined   |
| \_contents     | IAirdropERC1155.AirdropContent[] | undefined   |

### airdrop

```solidity
function airdrop(uint256 paymentsToProcess) external nonpayable
```

Lets contract-owner send ERC721 NFTs to a list of addresses.

#### Parameters

| Name              | Type    | Description |
| ----------------- | ------- | ----------- |
| paymentsToProcess | uint256 | undefined   |

### contractType

```solidity
function contractType() external pure returns (bytes32)
```

_Returns the type of the contract._

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | bytes32 | undefined   |

### contractVersion

```solidity
function contractVersion() external pure returns (uint8)
```

_Returns the version of the contract._

#### Returns

| Name | Type  | Description |
| ---- | ----- | ----------- |
| \_0  | uint8 | undefined   |

### getAllAirdropPayments

```solidity
function getAllAirdropPayments() external view returns (struct IAirdropERC1155.AirdropContent[] contents)
```

Returns all airdrop payments set up -- pending, processed or failed.

#### Returns

| Name     | Type                             | Description |
| -------- | -------------------------------- | ----------- |
| contents | IAirdropERC1155.AirdropContent[] | undefined   |

### getAllAirdropPaymentsFailed

```solidity
function getAllAirdropPaymentsFailed() external view returns (struct IAirdropERC1155.AirdropContent[] contents)
```

Returns all pending airdrop failed.

#### Returns

| Name     | Type                             | Description |
| -------- | -------------------------------- | ----------- |
| contents | IAirdropERC1155.AirdropContent[] | undefined   |

### getAllAirdropPaymentsPending

```solidity
function getAllAirdropPaymentsPending() external view returns (struct IAirdropERC1155.AirdropContent[] contents)
```

Returns all pending airdrop payments.

#### Returns

| Name     | Type                             | Description |
| -------- | -------------------------------- | ----------- |
| contents | IAirdropERC1155.AirdropContent[] | undefined   |

### getAllAirdropPaymentsProcessed

```solidity
function getAllAirdropPaymentsProcessed() external view returns (struct IAirdropERC1155.AirdropContent[] contents)
```

Returns all pending airdrop processed.

#### Returns

| Name     | Type                             | Description |
| -------- | -------------------------------- | ----------- |
| contents | IAirdropERC1155.AirdropContent[] | undefined   |

### getRoleAdmin

```solidity
function getRoleAdmin(bytes32 role) external view returns (bytes32)
```

Returns the admin role that controls the specified role.

_See {grantRole} and {revokeRole}. To change a role&#39;s admin, use {\_setRoleAdmin}._

#### Parameters

| Name | Type    | Description                                                           |
| ---- | ------- | --------------------------------------------------------------------- |
| role | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | bytes32 | undefined   |

### getRoleMember

```solidity
function getRoleMember(bytes32 role, uint256 index) external view returns (address member)
```

Returns the role-member from a list of members for a role, at a given index.

_Returns `member` who has `role`, at `index` of role-members list. See struct {RoleMembers}, and mapping {roleMembers}_

#### Parameters

| Name  | Type    | Description                                                           |
| ----- | ------- | --------------------------------------------------------------------- |
| role  | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |
| index | uint256 | Index in list of current members for the role.                        |

#### Returns

| Name   | Type    | Description                        |
| ------ | ------- | ---------------------------------- |
| member | address | Address of account that has `role` |

### getRoleMemberCount

```solidity
function getRoleMemberCount(bytes32 role) external view returns (uint256 count)
```

Returns total number of accounts that have a role.

_Returns `count` of accounts that have `role`. See struct {RoleMembers}, and mapping {roleMembers}_

#### Parameters

| Name | Type    | Description                                                           |
| ---- | ------- | --------------------------------------------------------------------- |
| role | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |

#### Returns

| Name  | Type    | Description                               |
| ----- | ------- | ----------------------------------------- |
| count | uint256 | Total number of accounts that have `role` |

### grantRole

```solidity
function grantRole(bytes32 role, address account) external nonpayable
```

Grants a role to an account, if not previously granted.

_Caller must have admin role for the `role`. Emits {RoleGranted Event}._

#### Parameters

| Name    | Type    | Description                                                           |
| ------- | ------- | --------------------------------------------------------------------- |
| role    | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |
| account | address | Address of the account to which the role is being granted.            |

### hasRole

```solidity
function hasRole(bytes32 role, address account) external view returns (bool)
```

Checks whether an account has a particular role.

_Returns `true` if `account` has been granted `role`._

#### Parameters

| Name    | Type    | Description                                                           |
| ------- | ------- | --------------------------------------------------------------------- |
| role    | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |
| account | address | Address of the account for which the role is being checked.           |

#### Returns

| Name | Type | Description |
| ---- | ---- | ----------- |
| \_0  | bool | undefined   |

### hasRoleWithSwitch

```solidity
function hasRoleWithSwitch(bytes32 role, address account) external view returns (bool)
```

Checks whether an account has a particular role; role restrictions can be switched on and off.

_Returns `true` if `account` has been granted `role`. Role restrictions can be switched on and off: - If address(0) has ROLE, then the ROLE restrictions don&#39;t apply. - If address(0) does not have ROLE, then the ROLE restrictions will apply._

#### Parameters

| Name    | Type    | Description                                                           |
| ------- | ------- | --------------------------------------------------------------------- |
| role    | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |
| account | address | Address of the account for which the role is being checked.           |

#### Returns

| Name | Type | Description |
| ---- | ---- | ----------- |
| \_0  | bool | undefined   |

### initialize

```solidity
function initialize(address _defaultAdmin) external nonpayable
```

_Initializes the contract, like a constructor._

#### Parameters

| Name           | Type    | Description |
| -------------- | ------- | ----------- |
| \_defaultAdmin | address | undefined   |

### multicall

```solidity
function multicall(bytes[] data) external nonpayable returns (bytes[] results)
```

_Receives and executes a batch of function calls on this contract._

#### Parameters

| Name | Type    | Description |
| ---- | ------- | ----------- |
| data | bytes[] | undefined   |

#### Returns

| Name    | Type    | Description |
| ------- | ------- | ----------- |
| results | bytes[] | undefined   |

### owner

```solidity
function owner() external view returns (address)
```

Returns the owner of the contract.

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | address | undefined   |

### payeeCount

```solidity
function payeeCount() external view returns (uint256)
```

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | uint256 | undefined   |

### processedCount

```solidity
function processedCount() external view returns (uint256)
```

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | uint256 | undefined   |

### renounceRole

```solidity
function renounceRole(bytes32 role, address account) external nonpayable
```

Revokes role from the account.

_Caller must have the `role`, with caller being the same as `account`. Emits {RoleRevoked Event}._

#### Parameters

| Name    | Type    | Description                                                           |
| ------- | ------- | --------------------------------------------------------------------- |
| role    | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |
| account | address | Address of the account from which the role is being revoked.          |

### revokeRole

```solidity
function revokeRole(bytes32 role, address account) external nonpayable
```

Revokes role from an account.

_Caller must have admin role for the `role`. Emits {RoleRevoked Event}._

#### Parameters

| Name    | Type    | Description                                                           |
| ------- | ------- | --------------------------------------------------------------------- |
| role    | bytes32 | keccak256 hash of the role. e.g. keccak256(&quot;TRANSFER_ROLE&quot;) |
| account | address | Address of the account from which the role is being revoked.          |

### setOwner

```solidity
function setOwner(address _newOwner) external nonpayable
```

Lets an authorized wallet set a new owner for the contract.

#### Parameters

| Name       | Type    | Description                                          |
| ---------- | ------- | ---------------------------------------------------- |
| \_newOwner | address | The address to set as the new owner of the contract. |

## Events

### AirdropPayment

```solidity
event AirdropPayment(address indexed recipient, IAirdropERC1155.AirdropContent content)
```

Emitted when an airdrop payment is made to a recipient.

#### Parameters

| Name                | Type                           | Description |
| ------------------- | ------------------------------ | ----------- |
| recipient `indexed` | address                        | undefined   |
| content             | IAirdropERC1155.AirdropContent | undefined   |

### Initialized

```solidity
event Initialized(uint8 version)
```

#### Parameters

| Name    | Type  | Description |
| ------- | ----- | ----------- |
| version | uint8 | undefined   |

### OwnerUpdated

```solidity
event OwnerUpdated(address indexed prevOwner, address indexed newOwner)
```

#### Parameters

| Name                | Type    | Description |
| ------------------- | ------- | ----------- |
| prevOwner `indexed` | address | undefined   |
| newOwner `indexed`  | address | undefined   |

### RecipientsAdded

```solidity
event RecipientsAdded(IAirdropERC1155.AirdropContent[] _contents)
```

Emitted when airdrop recipients are uploaded to the contract.

#### Parameters

| Name       | Type                             | Description |
| ---------- | -------------------------------- | ----------- |
| \_contents | IAirdropERC1155.AirdropContent[] | undefined   |

### RoleAdminChanged

```solidity
event RoleAdminChanged(bytes32 indexed role, bytes32 indexed previousAdminRole, bytes32 indexed newAdminRole)
```

#### Parameters

| Name                        | Type    | Description |
| --------------------------- | ------- | ----------- |
| role `indexed`              | bytes32 | undefined   |
| previousAdminRole `indexed` | bytes32 | undefined   |
| newAdminRole `indexed`      | bytes32 | undefined   |

### RoleGranted

```solidity
event RoleGranted(bytes32 indexed role, address indexed account, address indexed sender)
```

#### Parameters

| Name              | Type    | Description |
| ----------------- | ------- | ----------- |
| role `indexed`    | bytes32 | undefined   |
| account `indexed` | address | undefined   |
| sender `indexed`  | address | undefined   |

### RoleRevoked

```solidity
event RoleRevoked(bytes32 indexed role, address indexed account, address indexed sender)
```

#### Parameters

| Name              | Type    | Description |
| ----------------- | ------- | ----------- |
| role `indexed`    | bytes32 | undefined   |
| account `indexed` | address | undefined   |
| sender `indexed`  | address | undefined   |
