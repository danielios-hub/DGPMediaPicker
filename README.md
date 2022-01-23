# Media Picker 

## BDD Specs

### Story: Take a photo from the camera

### Narrative 1: 

```
As an user
I want to take an image from the camera
```


#### Scenarios (acceptance criteria) 
```
Given the user has camera permissions
When the user take a photo
Then the app return an image with the photo
```

```
Given the user has no camera permissions
When the user try to take a photo
Then the app display an option to give permission
```

### Story: Photo Gallery

### Narrative 1: 
```
As an user
I want to visualize and select photos from the photos app
```

#### Scenarios: 
```
Given the user has permission to photo app
When the user request to see all photos from the library app
Then the app display a list of all photos
```

```
Given the user does not has permission to photo app
When the user request to see all photos from the library app
Then the app display an option to give permissions
```


## Use cases

## Take a single photo

### Primary course:
1. System ask for permission to access the camera
2. User agree to give permission
3. Camera become active
4. User take a photo
5. System return the taken image

### No permissions: 
1. System display a way for requesting for permission again

### Failure taken a photo (if aplicable):
1: System display an error message


## Load all images from photo app

### Primary course: 
1. System ask for permission to access the photo app library
2. User agree to give permission
3. System display all images

### Secondary course: 
4. System display a way to change album from photo app
5. User change album
6. System display all images from the selected album

### No permissions: 
1. System display a way for requesting for permission again

### Failure loading photos
1: System display an error message and give an option for loading again


## Select an image from the photo app

### Data: 
- Photos are already loaded and display

### Primary course: 
1. User select a photo
2. System return selected image


