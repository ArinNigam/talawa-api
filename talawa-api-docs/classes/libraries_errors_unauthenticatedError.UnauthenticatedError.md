[talawa-api](../README.md) / [Exports](../modules.md) / [libraries/errors/unauthenticatedError](../modules/libraries_errors_unauthenticatedError.md) / UnauthenticatedError

# Class: UnauthenticatedError

[libraries/errors/unauthenticatedError](../modules/libraries_errors_unauthenticatedError.md).UnauthenticatedError

This class detects unauthenticated errors and sends those errors to the superclass ApplicationError.

## Hierarchy

- [`ApplicationError`](libraries_errors_applicationError.ApplicationError.md)

  ↳ **`UnauthenticatedError`**

## Table of contents

### Constructors

- [constructor](libraries_errors_unauthenticatedError.UnauthenticatedError.md#constructor)

### Properties

- [errors](libraries_errors_unauthenticatedError.UnauthenticatedError.md#errors)
- [httpCode](libraries_errors_unauthenticatedError.UnauthenticatedError.md#httpcode)
- [message](libraries_errors_unauthenticatedError.UnauthenticatedError.md#message)
- [name](libraries_errors_unauthenticatedError.UnauthenticatedError.md#name)
- [stack](libraries_errors_unauthenticatedError.UnauthenticatedError.md#stack)
- [prepareStackTrace](libraries_errors_unauthenticatedError.UnauthenticatedError.md#preparestacktrace)
- [stackTraceLimit](libraries_errors_unauthenticatedError.UnauthenticatedError.md#stacktracelimit)

### Methods

- [captureStackTrace](libraries_errors_unauthenticatedError.UnauthenticatedError.md#capturestacktrace)

## Constructors

### constructor

• **new UnauthenticatedError**(`message?`, `code?`, `param?`, `metadata?`): [`UnauthenticatedError`](libraries_errors_unauthenticatedError.UnauthenticatedError.md)

#### Parameters

| Name       | Type                     | Default value            |
| :--------- | :----------------------- | :----------------------- |
| `message`  | `string`                 | `"UnauthenticatedError"` |
| `code`     | `null` \| `string`       | `null`                   |
| `param`    | `null` \| `string`       | `null`                   |
| `metadata` | `Record`\<`any`, `any`\> | `\{\}`                   |

#### Returns

[`UnauthenticatedError`](libraries_errors_unauthenticatedError.UnauthenticatedError.md)

#### Overrides

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[constructor](libraries_errors_applicationError.ApplicationError.md#constructor)

#### Defined in

[src/libraries/errors/unauthenticatedError.ts:6](https://github.com/PalisadoesFoundation/talawa-api/blob/cf57ca9/src/libraries/errors/unauthenticatedError.ts#L6)

## Properties

### errors

• **errors**: [`InterfaceError`](../interfaces/libraries_errors_applicationError.InterfaceError.md)[]

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[errors](libraries_errors_applicationError.ApplicationError.md#errors)

#### Defined in

[src/libraries/errors/applicationError.ts:11](https://github.com/PalisadoesFoundation/talawa-api/blob/cf57ca9/src/libraries/errors/applicationError.ts#L11)

---

### httpCode

• **httpCode**: `number`

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[httpCode](libraries_errors_applicationError.ApplicationError.md#httpcode)

#### Defined in

[src/libraries/errors/applicationError.ts:12](https://github.com/PalisadoesFoundation/talawa-api/blob/cf57ca9/src/libraries/errors/applicationError.ts#L12)

---

### message

• **message**: `string`

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[message](libraries_errors_applicationError.ApplicationError.md#message)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1076

---

### name

• **name**: `string`

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[name](libraries_errors_applicationError.ApplicationError.md#name)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1075

---

### stack

• `Optional` **stack**: `string`

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[stack](libraries_errors_applicationError.ApplicationError.md#stack)

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1077

---

### prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) =\> `any`

Optional override for formatting stack traces

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

#### Type declaration

▸ (`err`, `stackTraces`): `any`

Optional override for formatting stack traces

##### Parameters

| Name          | Type         |
| :------------ | :----------- |
| `err`         | `Error`      |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[prepareStackTrace](libraries_errors_applicationError.ApplicationError.md#preparestacktrace)

#### Defined in

node_modules/@types/node/globals.d.ts:28

---

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[stackTraceLimit](libraries_errors_applicationError.ApplicationError.md#stacktracelimit)

#### Defined in

node_modules/@types/node/globals.d.ts:30

## Methods

### captureStackTrace

▸ **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name              | Type       |
| :---------------- | :--------- |
| `targetObject`    | `object`   |
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

[ApplicationError](libraries_errors_applicationError.ApplicationError.md).[captureStackTrace](libraries_errors_applicationError.ApplicationError.md#capturestacktrace)

#### Defined in

node_modules/@types/node/globals.d.ts:21