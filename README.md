# SAP Fiori Standalone App URL Generator

A simple browser-based tool to generate URLs for running SAP Fiori apps in standalone mode (without full Launchpad navigation).

## What it does

Generates URLs using the `#Shell-runStandaloneApp` intent format:

```
https://<server>:<port>/sap/bc/ui5_ui5/ui2/ushell/shells/abap/FioriLaunchpad.html?sap-client=<client>&sap-ushell-config=<config>#Shell-runStandaloneApp?sap-ushell-SAPUI5.Component=<component>&sap-ushell-url=<app-path>
```

## Features

- Generate standalone Fiori app URLs with proper encoding
- Copy to clipboard with one click
- Brief explanations for each input field
- Support for app-specific startup parameters
- No dependencies — single HTML file, works offline

## Target Users

ABAP developers who maintain and configure SAP Fiori applications.

## Usage

1. Open `index.html` in any browser, or visit the [GitHub Pages deployment](https://<your-username>.github.io/<repo-name>/)
2. Fill in your system details (server, port, client, etc.)
3. Enter the SAPUI5 component name and BSP application path
4. Click **Generate URL**
5. Click **Copy URL** to copy to clipboard

## Deploy to GitHub Pages

1. Create a new repository on GitHub
2. Push this folder to the repository
3. Go to Settings → Pages → Source: Deploy from branch (main, root)
4. Your tool will be live at `https://<username>.github.io/<repo-name>/`

## Note

The `#Shell-runStandaloneApp` intent was deprecated in UI Add-On for SAP NetWeaver 2.0+. This tool is still useful for older systems or specific standalone/headerless use cases.

## Reference

- [SAP Help - Running a Standalone Application](https://help.sap.com/saphelp_em92/helpdata/de/53/7758e0deb0477386ea400c915073b3/content.htm)
- [SAP Help - UI Add-On for SAP NetWeaver](https://help.sap.com/docs/UI_ADD-ON_FOR_SAP_NETWEAVER_20/17ae0e97e0fc424a9c368f350c0ba6bd)

## License

MIT
