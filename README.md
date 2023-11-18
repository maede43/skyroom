# Skyroom

A Node.js wrapper for the Skyroom online education API

## Table of Contents

- [Getting started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Versioning](#versioning)
- [Authors](#authors)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Getting Started

This project is a Node.js wrapper dedicated to interfacing with the Skyroom online teaching and learning system using the Skyroom API. Skyroom offers robust features for facilitating online education and this module makes it easy to interact with their platform from your Node.js projects. 

### Prerequisites

Ensure you have Node.js installed on your local machine to be able to use this wrapper effectively. You can check your Node.js installation by running `node -v` in your terminal. If you do not have Node.js installed, you can download it [here](https://nodejs.org/en/download/).

Before using this wrapper, you will need to obtain an API key from the Skyroom website. This requires a valid account on the platform. To access, link, and manage your Skyroom web services, you will use this API key.

## Installation

To install the Skyroom package, you'll need to have [npm](https://www.npmjs.com/get-npm) (Node Package Manager) installed. 

You can install the package via NPM using the following command in your terminal:

```bash
npm install skyroom
```

## Usage

Below is an example of how to use the package:

```javascript
const Skyroom = require('skyroom');
const skyroom = new Skyroom('<YOUR_SKYROOM_API_KEY>');

const params = {
    user_id: '<USER_ID>',
    user_nick: '<NICKNAME>',
};

skyroom.getUser(params).then((response)=>{
    console.log(response);
}).catch((e)=>{
    console.log(e);
});
```

## Contributing

If you have any ideas, just [open an issue](https://github.com/maede43/skyroom/issues/new) and tell us what you think.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are warmly welcome.

## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, Skyroom is maintained under the Semantic Versioning guidelines.

See the [Releases section](https://github.com/maede43/skyroom/releases) of our GitHub project for changelogs for each release version.

## Authors

- **Mohammad Hossein Hosseini** - [smhhoseinee](https://github.com/smhhoseinee)
- **Maedeh Nadehi**  - [maede43](https://github.com/maede43)
- **MohammadMohammadZadehKalati**  - [MohammadMohammadZadehKalati](https://github.com/MohammadMohammadZadehKalati)

See also the list of [contributors](https://github.com/maede43/skyroom/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Thanks to Skyroom for providing the API
* Inspiration: To provide a great education tool
