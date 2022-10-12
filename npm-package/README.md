# Delivering the Payload as an NPM Package

1. Copy the compiled `providers.dll` into this directory.
1. For the sake of experimentation, we use a private NPM registry.
   **Do not upload malicious NPM packages to the official registry!**
   For example, if our private NPM registry can be found at https://npm.ianyong.com, we can set it as the NPM registry to use by default via:
   ```
   npm set registry https://npm.ianyong.com
   ```
   Alternatively, we can append every command that involves the registry with:
   ```
   --registry https://npm.ianyong.com
   ```
1. Login to the private NPM registry:
   ```
   npm login
   ```
1. Publish the NPM package:
   ```
   npm publish
   ```
