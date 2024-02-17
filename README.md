# DATABASE SCRIPTING

This is me learning how to write scripts that can modify MongoDB schema and data.  
Two types of schemas are written in this application referencing one MongoDB collection.  
The idea is to able to change the collection data with reverse possibility.   
You can create users with an option to set the visibility of their `email, phone, and country` or as strings with no visibility option. The visibility options can be `Private, Everyone, or Administrators`.

## Setup

Clone the repository.    
cd into the project directory          
Run `yarn install` or `npm install`    
Create a `.env` file and add your database URL there (check `.env.example` for guidance) 

### Usage

- To populate data in MongoDB with no option for visibility settings:  
  `yarn run add-users-to-db` OR `npm run add-users-to-db`

- To populate data in MongoDB with an option for visibility settings:  
  `yarn run add-users-with-visibility-to-db` OR `npm run add-users-with-visibility-to-db`

- To reformat data in MongoDB with no option for visibility settings:  
`yarn run execute-scripts removeVisibilitySettingsFromUserData` OR `npm run execute-scripts removeVisibilitySettingsFromUserData `

- To reformat data in MongoDB with an option for visibility settings:  
`yarn run execute-scripts addVisibilitySettingsToUserData` OR `npm run execute-scripts addVisibilitySettingsToUserData `
