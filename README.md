# Setup Vulkan SDK

## Made by SpargatGroup.

## Informations of the project

### Latest release

![GitHub release (latest by date)](https://img.shields.io/github/v/release/SpargatTeam/setup-vulkan-sdk)

### Build status

[![Setup Vulkan SDK workflow build status](https://github.com/SpargatGroup/setup-vulkan-sdk/actions/workflows/test.yaml/badge.svg)](https://github.com/SpargatGroup/setup-vulkan-sdk/actions)

### You can see the extension on Marketplace [https://github.com/marketplace/actions/setup-vulkan-sdk-multiplatform](here)

### Working perfect for Linux and Windows, good for macos but no components extra

## Usage example of the project

### For latest stable

``` yaml
      - name: Setup Vulkan SDK # action name
        uses: SpargatGroup/setup-vulkan-sdk@v1.0.0
        with:
          version: '1.3.296.0'  # Vulkan SDK version you want
          components: 'Vulkan-Headers,Vulkan-Loader'  # Vulkan components you need
          cache: 'true'  # Vulkan Cache
```

### For latest comit (unstable)

``` yaml
      - name: Setup Vulkan SDK # action name
        uses: SpargatGroup/setup-vulkan-sdk@latest
        with:
          version: 'latest'  # Vulkan SDK version you want
          components: 'Vulkan-Headers,Vulkan-Loader'  # Vulkan components you need
          cache: 'true'  # Vulkan Cache
```

## Test Vulkan SDK

### For download path

```bash
echo $VULKAN_SDK
```

### For version downloaded

```bash
echo $VERSION_VULKAN_TO_DOWNLOAD
```