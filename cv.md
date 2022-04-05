# Andrey Pokrovsky
Web developer

## About me
I started my career as a coder in a small web studio with a friend of mine. Back then, I didn’t fully understand how websites worked, and I really wanted to understand it. I started learning PHP and then WordPress, got a job at a university where I developed a site on this CMS. Working at the university helped me develop and consolidate the necessary skills, after which I decided to increase my level of income and changed jobs twice until I found a company where I have been working for almost a Ёyear.

All this time, I was not sure in which direction I wanted to develop, so I started experimenting with various technologies: Java, Python, etc. As a result, I realized that I like JavaScript the most. Now I'm studying frontend, and after that I plan to study backend on NodeJS, because in the future I want to become an IT entrepreneur and create my own products.

## Contacts
- Phone: +7 965 165 08 88
- E-mail: iampokrovsky@gmail.com
- Telegram: @iampokrovsky

## Knowledge and skills

**Knowledges:**
- HTML 5
- CSS 3
- BEM
- Bootstrap
- JavaScript
- Gulp
- Pug (Jade)
- PHP
- Bitrix
- WordPress
- Git and GitHub
- Figma
- Adobe Photoshop

**Skills:**
- Adaptive cross-browser valid layout using BEM methodology
- Developing interactive modules and simple web applications using JavaScript
- Using build systems in the work, writing instructions for t~~heir operation
- Using the Git version control system and the GitHub
- Design of individual elements of the user interface using a common design concept
- Connecting and configuring ready-made modules and libraries
- Optimizing website performance
- Development of technical specifications for the site
- Reading technical documentation in English
- Improving the accessibility of web pages for people with disabilities
- Form creation and processing
- Website administration, content filling
- Optimization of the code of existing projects
- Photo processing and optimization
- Creating the necessary visual content using the editors Adobe Photoshop and Figma
- Connecting ready-made web pages to a content management system

## Work experience
- October 2019 - June 2020 - Ivan Sokolov web studio
- June 2020 - March 2021 - State University of Management, Moscow
- March 2021 - June 2021 - Moscow Aviation Institute
- June 2021 - until now - Moscow Center of Dental Implantology ROOTT

## Education
- HTML Academy HTML, CSS and JavaScript interactive courses
- HTML Academy JavaScript course, level 1
- HTML Academy JavaScript course, level 2
- HTML Academy PHP course, level 1
- LoftSchool WordPress course
- WebForMyself 1C-Bitrix course
- JavaScript course for programmers by JavaScript.ru

## Languages
- Russian - Native
- English - B1

## Code example
The solution of the [Human readable duration format](https://www.codewars.com/kata/human-readable-duration-format) problem on Codewars:
```
function formatDuration(seconds) {
  if (seconds === 0) return 'now';

  const units = [
    ['second', 60],
    ['minute', 60],
    ['hour', 24],
    ['day', 365],
    ['year', seconds],
  ];

  return units
    .reduce((result, [unit, measure]) => {
      let rest = seconds % measure;
      seconds = (seconds - rest) / measure;
      let title = unit + (rest > 1 ? 's' : '');

      if (rest > 0) result.push(`${rest} ${title}`);

      return result;
    }, [])
    .reverse()
    .join(', ')
    .replace(/(, )(?!.*, )/gi, ' and ');
}
```