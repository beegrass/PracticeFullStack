# PracticeFullStack
Follows the full stack development course with Java, Spring Boot, MongoDB, and PostgreSQL. Taught by Get Arrays on YouTube

# To Run
## Dependencies
- Latest version of NodeJS or similar
- Latest version of Java
- Latest version of PostgreSQL
**Note: The latest versions aren't actually necessary but it's what I used and ensures there's no issues.**

## API Backend
1. Open a terminal in the project
2. From the root directory, cd into the `contactapi` directory
3. Copy and run the command: `mvn spring-boot:run`
- This will spin up the backend with Spring Boot. You should see something like `Started Application in xyz seconds` if it worked

## Vite React Frontend
1. Open a second terminal in the project
2. From the root directory, cd into the `contactapp` directory
3. Copy and run the command: `npm run dev`
- This will start the dev server. You should see something like `Local: http://localhost:xxxx` where `xxxx` is four digits. Click this link to view the website.
**Note: your website may show at a different link and it may be necessary to add it to the CORS allowed origins. Follow [these steps](#add-to-cors-allowed-origins) if this happens to you**

### Add To Cors Allowed Origins
1. Open the `contactapi` directory
2. Navigate to `src\main\java\com\practice\contactapi\config\CorsConfig.java`
3. On line 35 where there is a List of allowed origins, add yours to the list
4. Save and rerun the command to spin up the backend