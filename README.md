<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-fireworks 1.2.1

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-fireworks.git", from: "1.2.1")
```

Products: `SwiftAIFireworks`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Fireworks AI for Swift

`SwiftAIFireworks` adds Fireworks AI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/fireworks` and supports text generation, text completion, embeddings and image generation.

Provider guide with models, options, streaming and errors:

- [Fireworks AI](https://swiftaisdk.github.io/SwiftAISDK/providers/fireworks/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIFireworks` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIFireworks

let provider = try AIProviders.fireworks(configuration: FireworksProviderSettings())
```

By default the provider reads `FIREWORKS_API_KEY` from the environment; values set in `FireworksProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-fireworks` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
