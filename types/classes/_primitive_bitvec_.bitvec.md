[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["primitive/BitVec"](../modules/_primitive_bitvec_.md) › [BitVec](_primitive_bitvec_.bitvec.md)

# Class: BitVec

**`name`** BitVec

**`description`** 
A BitVec that represents an array of bits. The bits are however stored encoded. The difference between this
and a normal Bytes would be that the length prefix indicates the number of bits encoded, not the bytes

## Hierarchy

  ↳ [Raw](_codec_raw_.raw.md)

  ↳ **BitVec**

## Implements

* [IU8a](../interfaces/_types_interfaces_.iu8a.md)

## Indexable

* \[ **index**: *number*\]: number

**`name`** BitVec

**`description`** 
A BitVec that represents an array of bits. The bits are however stored encoded. The difference between this
and a normal Bytes would be that the length prefix indicates the number of bits encoded, not the bytes

## Index

### Constructors

* [constructor](_primitive_bitvec_.bitvec.md#constructor)

### Properties

* [registry](_primitive_bitvec_.bitvec.md#registry)

### Accessors

* [encodedLength](_primitive_bitvec_.bitvec.md#encodedlength)
* [hash](_primitive_bitvec_.bitvec.md#hash)
* [isEmpty](_primitive_bitvec_.bitvec.md#isempty)
* [length](_primitive_bitvec_.bitvec.md#length)

### Methods

* [bitLength](_primitive_bitvec_.bitvec.md#bitlength)
* [eq](_primitive_bitvec_.bitvec.md#eq)
* [subarray](_primitive_bitvec_.bitvec.md#subarray)
* [toHex](_primitive_bitvec_.bitvec.md#tohex)
* [toHuman](_primitive_bitvec_.bitvec.md#tohuman)
* [toJSON](_primitive_bitvec_.bitvec.md#tojson)
* [toRawType](_primitive_bitvec_.bitvec.md#torawtype)
* [toString](_primitive_bitvec_.bitvec.md#tostring)
* [toU8a](_primitive_bitvec_.bitvec.md#tou8a)

## Constructors

###  constructor

\+ **new BitVec**(`registry`: [Registry](../interfaces/_types_registry_.registry.md), `value?`: [AnyU8a](../modules/_types_helpers_.md#anyu8a)): *[BitVec](_primitive_bitvec_.bitvec.md)*

*Overrides [Raw](_codec_raw_.raw.md).[constructor](_codec_raw_.raw.md#constructor)*

*Defined in [packages/types/src/primitive/BitVec.ts:42](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/primitive/BitVec.ts#L42)*

**Parameters:**

Name | Type |
------ | ------ |
`registry` | [Registry](../interfaces/_types_registry_.registry.md) |
`value?` | [AnyU8a](../modules/_types_helpers_.md#anyu8a) |

**Returns:** *[BitVec](_primitive_bitvec_.bitvec.md)*

## Properties

###  registry

• **registry**: *[Registry](../interfaces/_types_registry_.registry.md)*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md).[registry](../interfaces/_types_interfaces_.iu8a.md#registry)*

*Inherited from [Raw](_codec_raw_.raw.md).[registry](_codec_raw_.raw.md#registry)*

*Defined in [packages/types/src/codec/Raw.ts:30](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L30)*

## Accessors

###  encodedLength

• **get encodedLength**(): *number*

*Overrides [Raw](_codec_raw_.raw.md).[encodedLength](_codec_raw_.raw.md#encodedlength)*

*Defined in [packages/types/src/primitive/BitVec.ts:50](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/primitive/BitVec.ts#L50)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Raw](_codec_raw_.raw.md).[hash](_codec_raw_.raw.md#hash)*

*Defined in [packages/types/src/codec/Raw.ts:48](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L48)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Inherited from [Raw](_codec_raw_.raw.md).[isEmpty](_codec_raw_.raw.md#isempty)*

*Defined in [packages/types/src/codec/Raw.ts:55](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L55)*

**`description`** Returns true if the type wraps an empty/default all-0 value

**Returns:** *boolean*

___

###  length

• **get length**(): *number*

*Inherited from [Raw](_codec_raw_.raw.md).[length](_codec_raw_.raw.md#length)*

*Overrides [IU8a](../interfaces/_types_interfaces_.iu8a.md).[length](../interfaces/_types_interfaces_.iu8a.md#length)*

*Defined in [packages/types/src/codec/Raw.ts:62](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L62)*

**`description`** The length of the value

**Returns:** *number*

## Methods

###  bitLength

▸ **bitLength**(): *number*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_codec_raw_.raw.md).[bitLength](_codec_raw_.raw.md#bitlength)*

*Defined in [packages/types/src/codec/Raw.ts:70](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L70)*

**`description`** Returns the number of bits in the value

**Returns:** *number*

___

###  eq

▸ **eq**(`other?`: any): *boolean*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_codec_raw_.raw.md).[eq](_codec_raw_.raw.md#eq)*

*Defined in [packages/types/src/codec/Raw.ts:77](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L77)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | any |

**Returns:** *boolean*

___

###  subarray

▸ **subarray**(`begin`: number, `end?`: undefined | number): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Raw](_codec_raw_.raw.md).[subarray](_codec_raw_.raw.md#subarray)*

*Overrides [IU8a](../interfaces/_types_interfaces_.iu8a.md).[subarray](../interfaces/_types_interfaces_.iu8a.md#subarray)*

*Defined in [packages/types/src/codec/Raw.ts:91](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L91)*

**`description`** Create a new subarray from the actual buffer. This is needed for compat reasons since a new Uint8Array gets returned here

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`begin` | number | The position to start at |
`end?` | undefined &#124; number | The position to end at  |

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

___

###  toHex

▸ **toHex**(): *string*

*Inherited from [Raw](_codec_raw_.raw.md).[toHex](_codec_raw_.raw.md#tohex)*

*Defined in [packages/types/src/codec/Raw.ts:98](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L98)*

**`description`** Returns a hex string representation of the value

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(): *[AnyJson](../modules/_types_helpers_.md#anyjson)*

*Inherited from [Raw](_codec_raw_.raw.md).[toHuman](_codec_raw_.raw.md#tohuman)*

*Defined in [packages/types/src/codec/Raw.ts:105](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L105)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Returns:** *[AnyJson](../modules/_types_helpers_.md#anyjson)*

___

###  toJSON

▸ **toJSON**(): *string*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_codec_raw_.raw.md).[toJSON](_codec_raw_.raw.md#tojson)*

*Defined in [packages/types/src/codec/Raw.ts:112](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L112)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *string*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Overrides [Raw](_codec_raw_.raw.md).[toRawType](_codec_raw_.raw.md#torawtype)*

*Defined in [packages/types/src/primitive/BitVec.ts:57](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/primitive/BitVec.ts#L57)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [IU8a](../interfaces/_types_interfaces_.iu8a.md)*

*Inherited from [Raw](_codec_raw_.raw.md).[toString](_codec_raw_.raw.md#tostring)*

*Overrides [IU8a](../interfaces/_types_interfaces_.iu8a.md).[toString](../interfaces/_types_interfaces_.iu8a.md#tostring)*

*Defined in [packages/types/src/codec/Raw.ts:126](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/codec/Raw.ts#L126)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Overrides [Raw](_codec_raw_.raw.md).[toU8a](_codec_raw_.raw.md#tou8a)*

*Defined in [packages/types/src/primitive/BitVec.ts:65](https://github.com/polkadot-js/api/blob/62f46359e/packages/types/src/primitive/BitVec.ts#L65)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value has none of the type-specific prefixes (internal)  |

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*