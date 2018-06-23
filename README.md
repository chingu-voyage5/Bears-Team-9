# Bears-Team-9

## Reffub
### The Buffer Clone

The overall objective of this project is to clone [Buffer](https://buffer.com/).  

The first part of the objective is to develop ability to post something to a single API (Yet to be determined which social media we will be selecting).

This will consistue as a MVP's objective:
1. Set up [MERN stack](https://github.com/Hashnode/mern-starter) to handle all aspects of the project.  The code below is a quick reference for macOS to get a MERN starter up and running in short order.
```
git clone https://github.com/Hashnode/mern-starter.git
cd mern-starter
npm install
brew update 
brew install mongodb
brew services start mongodb 
npm start
```
2. Create a backend to handle user's account information and API
    
    1. This requires a test website to be deployed to obtain necessary keys for API requests and testing.
    
3. Create a usable frontend for user to post to their selected social media.
    

## Masterminds behind this project:

### Miguel T Rivera 

I'm interested in learning Python for data science. I'm using the MERN stack currently for the advanced FCC projects.
I'm going to implement Marko for some of my projects instead of React.

Hi my name is Miguel T Rivera. I'm from Nor Cal (Northern California) and member of the freeCodeCamp Sacramento Meetup group.

*Coding Background*
I started with HTML in the late 90's. At a local community college, did a lot of C++, a little bit of Java and one semester of Python. Went to 4-year university to study Computer Science but I had a bad teacher, so I changed my major. In 2016, got back into programing through the freeCodeCamp program. I completed the front-end portion in Oct 2017. Currently, going through the full-stack application and data visualization certifications.

*Goals*
- Complete a team project
- Pair program
- Learn Python and dabble in data science
- Get more comfortable with React
- Get a developer job


### Luis Jimenez	
I was born and raised in Mexico City until the age of 13, when I moved to Texas, where I still currently live. I’m 19 years old, finished my third year in college (B.S. in Pure Mathematics and a Certificate in Numerical Analysis).
Coding: I started programming when I started college. I did a semester of Java and two semesters in C and parallel programming. I then started self-teaching web dev HTML, CSS and Vanilla JS and eventually did a lot of PHP. Recently I’ve built a couple of small websites for relatives using Laravel (PHP framework) and MySQL for backend and html, css and Vue for front end.
I’m comfortable with git, the Linux environment, ES6, webpack, SASS. This past semester I had an algorithms and software design class using Python, so I’d be okay with using that for the project.

### Paul Shreeman 
 
#### Team Leader for this project

 Ph.D in Nanoscale Science and Engineering specializing in modeling and algorithms to model X-Ray diffraction of thin-film semiconductors.  
 
 - [Linkedin](https://linkedin.com/in/pkshreeman)
 - [Stackoverflow](https://stackoverflow.com/story/pkshreeman)
 - [Github](https://github.com/pkshreeman)

 ### Issues

Issue: Travis CI build failure

Solution (by Miguel T Rivera):

1. Analyzed the build log and noticed it could not recognize ES6 syntax.
2. Decided it was probably old and that files needed to be updated.
3. Noticed some files were updated recently and others were 2 years old.
4. Tried updating the files using git but ran into issues.
5. Manually replaced/added old files with recent versions:

| Filename                      | Created? | Updated? | Location                  |
|-------------------------------|----------|----------|---------------------------|
| .dockerignore                 | Y        | N        | root                      |
| .gitignore                    | N        | Y        | root                      |
| .travis.yml                   | N        | Y        | root                      |
| Changes.md                    | Y        | N        | root                      |
| Dockerfile                    | N        | Y        | root                      |
| App.js                        | N        | Y        | /client/modules/App/      |
| store.js                      | N        | Y        | /client/                  |
| docker-compose-production.yml | Y        | N        | root                      |
| package-lock.json             | Y        | N        | root                      |
| package.json                  | N        | Y        | root                      |
| post.spec.js                  | N        | Y        | /server/models/__tests__/ |
| server.js                     | N        | Y        | /server/                  |
| test-helpers.js               | N        | Y        | /server/util/             |
| webpack.config.babel.js       | N        | Y        | root                      |
| webpack.config.dev.js         | N        | Y        | root                      |
| webpack.config.prod.js        | N        | Y        | root                      |
| webpack.config.server.js      | N        | Y        | root                      |

6. Tested it out and it built successfully.
7. Submitted a PR to the Bear-Team-09 master repo. 