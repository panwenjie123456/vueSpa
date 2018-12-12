# Assignment 2 - Vue app - Automated development process.

Name: Wenjie Pan

Student No.:  20082269

## Overview.

...... The main page of the library management app contains multiple click buttons to go to various functions. There is a description of the app and a quick link to the new book page. The top link is the home page, the management page, and the new book page.........

## E2E Testing.

. . . 
+$ npx cypress run --spec cypress/integration/Book.spec.js
Manage Books page
    ✓ allows a book to be deleted (6345ms)
    ✓ allows a book to be edited (6860ms)
    ✓ Add amounts of books (13003ms)
  3 passing (27s)
+npx cypress run --spec cypress/integration/home-page.spec.js
Home page
    ✓ Shows a header (3095ms)
    Navigation bar
      ✓ Shows the required links (1138ms)
      ✓ Redirects when links are clicked (797ms)
  3 passing (5s)
+npx cypress run --spec cypress/integration/Newbook.spec.js 
 Newbook page
    ✓ allows a valid book to be submitted (5066ms)
    ✓ shows error messages for incomplete form fields (2153ms)
  2 passing (7s) 

## Continuous Integration.

. . . 

https://travis-ci.org/panwenjie123456/vueSpa

## Automated Deployment.

....  

http://jealous-police.surge.sh/

## Extra features.

. . . . Bundling + Source conytol + Published test results + Webpack +heroku :https://nmgb.herokuapp.com/ . . . . .

## Appendix.

. . . .

+$ npx cypress run
  (Run Starting)

  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ Cypress:    3.1.3                                                                              │
  │ Browser:    Electron 59 (headless)                                                             │
  │ Specs:      3 found (Book.spec.js, home-page.spec.js, Newbook.spec.js)                         │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘


────────────────────────────────────────────────────────────────────────────────────────────────────

  Running: Book.spec.js...                                                                 (1 of 3)


  Manage Books page
    ✓ allows a book to be deleted (6674ms)
    ✓ allows a book to be edited (9186ms)
    ✓ Add amounts of books (2230ms)


  3 passing (18s)


  (Results)

  ┌────────────────────────────┐
  │ Tests:        3            │
  │ Passing:      3            │
  │ Failing:      0            │
  │ Pending:      0            │
  │ Skipped:      0            │
  │ Screenshots:  0            │
  │ Video:        true         │
  │ Duration:     18 seconds   │
  │ Spec Ran:     Book.spec.js │
  └────────────────────────────┘


  (Video)

  - Started processing:   Compressing to 32 CRF
  - Finished processing:  /Users/apple/Desktop/webappdev/vueSPA/cypress/videos/Book.spec.js.mp4 (5 seconds)


────────────────────────────────────────────────────────────────────────────────────────────────────

  Running: home-page.spec.js...                                                            (2 of 3)


  Home page
    ✓ Shows a header (5960ms)
    Navigation bar
      ✓ Shows the required links (1704ms)
      ✓ Redirects when links are clicked (710ms)


  3 passing (9s)


  (Results)

  ┌─────────────────────────────────┐
  │ Tests:        3                 │
  │ Passing:      3                 │
  │ Failing:      0                 │
  │ Pending:      0                 │
  │ Skipped:      0                 │
  │ Screenshots:  0                 │
  │ Video:        true              │
  │ Duration:     8 seconds         │
  │ Spec Ran:     home-page.spec.js │
  └─────────────────────────────────┘


  (Video)

  - Started processing:   Compressing to 32 CRF
  - Finished processing:  /Users/apple/Desktop/webappdev/vueSPA/cypress/videos/home-page.spec.js.mp4 (1 second)


────────────────────────────────────────────────────────────────────────────────────────────────────

  Running: Newbook.spec.js...                                                              (3 of 3)


  Newbook page
    ✓ allows a valid book to be submitted (7560ms)
    ✓ shows error messages for incomplete form fields (2237ms)


  2 passing (10s)


  (Results)

  ┌───────────────────────────────┐
  │ Tests:        2               │
  │ Passing:      2               │
  │ Failing:      0               │
  │ Pending:      0               │
  │ Skipped:      0               │
  │ Screenshots:  0               │
  │ Video:        true            │
  │ Duration:     9 seconds       │
  │ Spec Ran:     Newbook.spec.js │
  └───────────────────────────────┘


  (Video)

  - Started processing:   Compressing to 32 CRF
  - Finished processing:  /Users/apple/Desktop/webappdev/vueSPA/cypress/videos/Newbook.spec.js.mp4 (2 seconds)


====================================================================================================

  (Run Finished)


      Spec                                                Tests  Passing  Failing  Pending  Skipped
  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ ✔ Book.spec.js                              00:18        3        3        -        -        - │
  ├────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ ✔ home-page.spec.js                         00:08        3        3        -        -        - │
  ├────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ ✔ Newbook.spec.js                           00:09        2        2        -        -        - │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘
    All specs passed!                           00:36        8        8        -        -        -


