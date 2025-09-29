# relayapp-html5-template

A RelayApp frontend template based on native HTML + JavaScript + CSS, built with Vue 3 UMD version and RelayClient, runs directly without Node.js environment.

## Features

- **API Demonstrations**: Complete RelayClient API call examples and result displays
- **Dynamic Forms**: Automatically generate input forms based on API configuration
- **Real-time Preview**: API call results displayed with real-time formatting
- **Component-based Architecture**: Clear code structure, easy to understand and extend

## Project Structure

```
RelayApp-HTML5-Template/
├── index.html              # Project entry file
├── js/
│   ├── vue.global.js       # Vue 3 UMD version
│   ├── menu.js             # API menu configuration
│   └── RelayClient.umd.js  # RelayClient library
├── css/
│   └── style.css           # Page styles
├── images/                 # Image resources
└── icon.png                # RelayApp icon
```

## Quick Start

```bash
git clone https://github.com/RelayX-Protocol/RelayApp-HTML5-Template.git
cd RelayApp-HTML5-Template
```

After downloading, you can directly develop your own RelayApp based on this template.

## Basic Usage

### Import RelayClient

```html
<script src="./js/relayx-api.umd.js"></script>
```

### Initialize and Call

```javascript
// Initialize
const relayx = new RelayClient();

// API call example
const response = await relayx.getLanguage();
console.log('Current language:', response.result);
```

### Output Directory Configuration

For production deployment, project files are output directly to the RelayApp address directory.

#### Build Output

```
{RELAYAPP_ADDRESS}/
├── index.html
├── js/
├── css/
├── images/
├── icon.png
└── ...
```

## Development Notes

- This template demonstrates the basic RelayApp development pattern
- All API calls have complete example code
- You can develop your own RelayApp directly based on this template
- Follows RelayApp development specifications, including the required `icon.png` file

## Documentation

For more API details, please refer to the [RelayApp Development Documentation](https://relayx.gitbook.io/docs/).

## License

MIT
