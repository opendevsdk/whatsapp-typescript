# Reference
## Flows
<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">createFlow</a>(wabaId, { ...params }) -> WhatsappSDK.CreateFlowResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new WhatsApp Flow under a WABA account.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.createFlow("wabaId", {
    name: "name",
    categories: ["SIGN_UP", "SIGN_UP"]
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**wabaId:** `string` — WhatsApp Business Account ID
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.CreateFlowRequestWrapper` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">updateFlowMetadata</a>(flowId, { ...params }) -> WhatsappSDK.UpdateFlowMetadataResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update name, categories, or endpoint URI of an existing flow.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.updateFlowMetadata("flowId");

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**flowId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.UpdateFlowMetadataRequestWrapper` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">listFlows</a>(wabaId) -> WhatsappSDK.GetManyFlowsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List all flows under a WABA account.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.listFlows("wabaId");

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**wabaId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">getFlow</a>(flowId, { ...params }) -> WhatsappSDK.FlowDetail</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Get a single flow by ID, optionally specifying fields.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.getFlow("flowId");

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**flowId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.GetFlowRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">deleteFlow</a>(flowId) -> WhatsappSDK.DeleteFlowResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a flow permanently.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.deleteFlow("flowId");

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**flowId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">updateFlowJson</a>(flowId, { ...params }) -> WhatsappSDK.UpdateFlowJsonResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Upload or replace the flow.json asset for a flow.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.updateFlowJson("flowId", {
    file: {
        "key": "value"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**flowId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.UpdateFlowJsonRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">getFlowPreview</a>(flowId, { ...params }) -> WhatsappSDK.FlowPreviewResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Get the web preview URL for a flow. The `fields` parameter controls whether the existing preview link is invalidated. The returned `preview_url` can then have interactive URL parameters (interactive, flow_token, flow_action, flow_action_payload, phone_number) appended by the caller.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.getFlowPreview("flowId", {
    fields: "preview.invalidate(false)"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**flowId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.GetFlowPreviewRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.<a href="/src/api/resources/flows/client/Client.ts">publishFlow</a>(flowId) -> WhatsappSDK.PublishFlowResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Publish a flow, making it available to send to users.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.flows.publishFlow("flowId");

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**flowId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `FlowsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Media
<details><summary><code>client.media.<a href="/src/api/resources/media/client/Client.ts">getMedia</a>(mediaId, { ...params }) -> WhatsappSDK.RetrieveMediaResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve media metadata (URL, mime type, size) by media ID.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.media.getMedia("mediaId");

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**mediaId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.GetMediaRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `MediaClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Messages
<details><summary><code>client.messages.<a href="/src/api/resources/messages/client/Client.ts">sendMessage</a>(numberId, { ...params }) -> WhatsappSDK.SendMessageResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Send a ssage (text, media, interactive, template, contacts, etc.)
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.messages.sendMessage("numberId", {
    messaging_product: "whatsapp",
    to: "to",
    type: "text"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**numberId:** `string` — one number ID
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.SendMessageRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `MessagesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.messages.<a href="/src/api/resources/messages/client/Client.ts">showTypingIndicator</a>(numberId, { ...params }) -> WhatsappSDK.ShowTypingIndicatorResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Show a "typing…" indicator to the recipient. Send this before sending the actual message for a more natural conversation flow.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.messages.showTypingIndicator("numberId", {
    messaging_product: "whatsapp",
    status: "read",
    message_id: "message_id",
    typing_indicator: {
        type: "text"
    }
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**numberId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.ShowTypingIndicatorRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `MessagesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Waba
<details><summary><code>client.waba.<a href="/src/api/resources/waba/client/Client.ts">uploadEncryptionKey</a>(numberId, { ...params }) -> void</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Upload the business public encryption key used for end-to-end encrypted WhatsApp Flows. Uses application/x-www-form-urlencoded content type.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.waba.uploadEncryptionKey("numberId", {
    business_public_key: "business_public_key"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**numberId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.UploadEncryptionRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WabaClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.waba.<a href="/src/api/resources/waba/client/Client.ts">registerNumber</a>(numberId, { ...params }) -> void</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a phone number with WhatsApp Cloud API.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.waba.registerNumber("numberId", {
    messaging_product: "whatsapp",
    pin: "pin"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**numberId:** `string` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `WhatsappSDK.RegisterNumberRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `WabaClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

