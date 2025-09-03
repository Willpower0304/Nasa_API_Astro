<img width="1384" height="808" alt="image" src="https://github.com/user-attachments/assets/4568e0f7-6380-4edb-a4cb-5e10a97c456e" />


# 🌌 Nasa API Astro 

A lightweight web app built with Astro that displays real-time astronomical data using NASA's API. Explore space imagery, asteroid information, and other cosmic data in a clean, modern interface.


## Features

- Astronomy Picture of the Day (APOD)
- Near-Earth Asteroid data
- Fast, responsive Astro-powered UI
- Minimalist and mobile-friendly design


## 🛠 Tech Stack

#### Core
- Astro - Static site generator
- JavaScript - Logic and API interactions
- CSS - Styling and responsive design

#### Tools & Hosting
- pnpm - Package manager
- Netlify - Deployment and hosting

#### APIs
- NASA Open APIs - Astronomical data source

## API Reference

#### Base URL
https://api.nasa.gov/



#### Authentication
##### All requests require an API key. Use either:
####

- Your NASA API key (via `import.meta.env.NASA_API_KEY`)
- Default demo key: `DEMO_KEY` (rate limited)

####  Endpoints Used
🌠 Astronomy Picture of the Day (APOD)
- Endpoint: /planetary/apod
- Method: GET

####  Query Parameters:


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `API_KEY` | `string` | **Required**. Your NASA API key |
| `count` | `number` | Number of APOD images to return (default: 1) |
| `thumbs` | `boolean` | Return thumbnail URL for videos (default: false)
 


#### Example Request:

```javascript
const res = await fetch(
  `https://api.nasa.gov/planetary/apod?api_key=${API_KEY}&count=4&thumbs=true`
);
const apods = await res.json();
```

#### Response:
Returns an array of APOD objects with image/video data, titles, explanations, and dates.




## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`NASA_API_KEY`


## Run Locally

Clone the project

```bash
  git clone https://github.com/Willpower0304/Nasa_API_Astro.git
```

Go to the project directory

```bash
  cd Nasa_API_Astro
```

Install dependencies

```bash
  pnpm install
```

Set up environment variables

```bash
  NASA_API_KEY=your_api_key_here
```

Start the server

```bash
  pnpm run dev
```

Open your browser
Navigate to http://localhost:4321 to view the application

### !Important

If you want to deploy this project on Netlify install the dependencies if not just ignore this part.

Install dependencies

```bash
  pnpm add @astrojs/netlify@^6.5.9
```


## 🚀 Deployment
This project is configured for easy deployment on Netlify:

Start the server

```bash
  pnpm run build
```

The build output will be in the dist/ folder, ready for deployment. go to https://app.netlify.com/drop to deploy the proyect on netlify.




## Documentation

[Documentation](https://linktodocumentation](https://deepwiki.com/Willpower0304/Nasa_API_Astro/1-nasa-api-astro-overview))


## Author

- [@Willpower0304](https://www.github.com/Willpower0304)


## Feedback

If you have any feedback, please reach out to us at espinozaw657@gmail.com


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://portfolio-william0304.netlify.app/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/william-espinoza-7687722ab/)


