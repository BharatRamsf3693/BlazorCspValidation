# Blazor CSP Validation Samples

Sample Blazor Web Apps demonstrating Static SSR, Interactive Server, Interactive WebAssembly, and Interactive Auto render modes for Content Security Policy (CSP) testing

## Prerequisites

Ensure the following software is installed before running the samples:

- .NET SDK: **11.0.100-preview.7.26381.103**
- Visual Studio 2026 Insiders: **[12023.133] Professional**

---

## Running the Samples in Debug Mode

The repository contains the following sample applications:

- `CspStaticSsrSample`
- `CspInteractiveServerSample`
- `CspInteractiveWasmSample`
- `CspInteractiveAutoSample`

### Steps

1. Open the desired sample project in **Visual Studio 2026 Insiders**.
2. Click the **Run** button (or press **F5**).
3. The application launches in the browser.

**Note:** After opening the CspInteractiveWasmSample and CspInteractiveAutoSample projects in Visual Studio 2026 Insiders, ensure that the Server project is set as the startup project.

### Expected Result

Open the browser's **Developer Tools** and navigate to the **Console** tab.

An **inline script CSP violation** should be displayed in the browser console.

---

## Running the Published Output

Published binaries are available in:

```text
Evidence\PublishedBinaries.zip
```

### Steps

1. Extract `Evidence\PublishedBinaries.zip`.
2. The extracted package contains the following published application folders:
   - `StaticSSR`
   - `InteractiveServer`
   - `InteractiveWasm`
   - `InteractiveAuto`
3. Open the desired sample folder.
4. Double-click the generated `.exe` file.
5. The application launches in the browser.

### Expected Result

Open the browser's **Developer Tools** and navigate to the **Console** tab.

An **inline script CSP violation** should be displayed in the browser console.

---

## Sample Mapping

| Sample Project | Published Output Folder |
|----------------|-------------------------|
| `CspStaticSsrSample` | `StaticSSR` |
| `CspInteractiveServerSample` | `InteractiveServer` |
| `CspInteractiveWasmSample` | `InteractiveWasm` |
| `CspInteractiveAutoSample` | `InteractiveAuto` |

---

## Verification

For each sample, verify the following:

- The application launches successfully.
- An inline script CSP violation is reported in the browser console.
- The issue is reproducible in both Debug and Published scenarios.
