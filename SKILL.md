# micronaut.http.client Skill

Use this skill to work with Norm module `micronaut.http.client` version 5. Use only declarations listed below.

## `micronaut.http.client`

Source: `BlockingHttpClient.norm`

### `BlockingHttpClient`

```norm
interface BlockingHttpClient extends Closeable, LifeCycle<BlockingHttpClient>
```

#### `close`

```norm
Void close()
```

Returns: `Void`

#### `retrieve`

```norm
String? retrieve(String? arg0)
```

Parameters:

- `arg0`: `String?`

Returns: `String?`

## `micronaut.http.client`

Source: `HttpClient.norm`

### `HttpClient`

```norm
interface HttpClient extends Closeable, LifeCycle<HttpClient>
```

#### `close`

```norm
Void close()
```

Returns: `Void`

#### `toBlocking`

```norm
BlockingHttpClient? toBlocking()
```

Returns: `BlockingHttpClient?`

### `httpClientCreate`

```norm
HttpClient? httpClientCreate(URL? arg0)
```

Parameters:

- `arg0`: `URL?`

Returns: `HttpClient?`

## `micronaut.http.client`

Source: `JavaArrays.norm`

### `JavaStringArray`

```norm
class JavaStringArray
```

#### `JavaStringArray`

```norm
JavaStringArray(JavaStringArrayBindingToken token)
```

Parameters:

- `token`: `JavaStringArrayBindingToken`

#### `size`

```norm
Integer size()
```

Returns: `Integer`

#### `get`

```norm
String? get(Integer index)
```

Parameters:

- `index`: `Integer`

Returns: `String?`

#### `set`

```norm
Void set(Integer index, String? value)
```

Parameters:

- `index`: `Integer`
- `value`: `String?`

Returns: `Void`

### `javaStringArrayNew`

```norm
JavaStringArray javaStringArrayNew(Integer size)
```

Parameters:

- `size`: `Integer`

Returns: `JavaStringArray`

## `micronaut.http.client.annotation`

Source: `annotation/Client.norm`

### `Client`

```norm
annotation Client implements PackageTarget, TypeTarget, FieldTarget, ConstructorTarget, FunctionTarget, ParameterTarget, LocalTarget, RuntimeRetention, ManagedImplementation
```

#### `alpnModes`

```norm
List<String> alpnModes
```

Type: `List<String>`

#### `definitionType`

```norm
ClientDefinitionType definitionType
```

Type: `ClientDefinitionType`

#### `id`

```norm
String id
```

Type: `String`

#### `path`

```norm
String path
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `Client`

```norm
Client(List<String>? alpnModes, ClientDefinitionType? definitionType, String? id, String? path, String? value)
```

Parameters:

- `alpnModes`: `List<String>?`
- `definitionType`: `ClientDefinitionType?`
- `id`: `String?`
- `path`: `String?`
- `value`: `String?`

## `micronaut.http.client.annotation`

Source: `annotation/ClientDefinitionType.norm`

### `ClientDefinitionType`

```norm
enum ClientDefinitionType
```

#### `CLIENT`

```norm
CLIENT
```

#### `SERVER`

```norm
SERVER
```

## `micronaut.http.client.io.micronaut.context`

Source: `io/micronaut/context/LifeCycle.norm`

### `LifeCycle`

```norm
interface LifeCycle<T extends LifeCycle<T>> extends Closeable, AutoCloseable
```

Type parameters:

- `T` extends `LifeCycle<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`


