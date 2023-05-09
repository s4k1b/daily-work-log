Feb 11, 2021
------------
- Refactor ui builder json loader function, take url and request object and request method as input from paramter, pass these parameters from create and edit wizard pages.
- Writing MongoDB Ops Request JSONs

Feb 12, 2021
------------
- Write MongoDB Ops request JSONS for basic Upgrade operation
- Publish these ops jsons in ui-wizards repo
- Integrate api calls to fetch these jsons and create mongo-db-ops instance from console
- Use older delete apis and edit page for wizards without options step

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Feb 15, 2021
------------
- Review PR by mohin ragarding long strings inside key value input form component.
- Add functionality (edit, delete, disable, require) logic to the show more modal inside key value input form component.
- Integrate pages api, show tabs based on the pages response.
- Use pages api to get target resources in basic page.
- Fix console errors in ResourceViewer page

Feb 16, 2021
------------
- Add generic pages route, show generic resource inner tables in generic pages route,
- Call pages api only when required (when user, cluster, group, version or resource changes)
- Add create button on generic resource inner tables, navigate to appropriate create pages by passing necessary parameters and queries
- Pass route as context in ui-builder
- Initialize namespace and database ref from route query in MongoDBOps Create page

Feb 17, 2021
------------
- Distinguish data fetching logic for individual computed, api calls, on change and condition resolving, solves element not showing loader when computed resolves before api calls.
- MR review of Junayed, update and release master with lastest fixes. (release branch release-0.2.1)
- Discuss with Emruz vai about stash backup configuration create wizard
- Start writing ui json for stash backup configuration create wizard

Feb 18, 2021
------------
- Complete form for appbinding backup configuration
- Debug resource create issue (Linode api problem)
- Debug backup configuration not showing in mongodb resource backup tab

Feb 19, 2021
------------
- Add logic (compute function) to initialize target ref in backup configuration wizard from router query params.
- Add functionality to backup configuration wizard json to modify structure of model json on target ref change
- Integrate console-config complete api, adjust compatibity with new response for console-config
- Integrate logic to show not installed banner when resource is not installed in cluster, in GenericInnerTable
- Setup gitea and ui-builder-demo cluster for mohin to fix some styles
- Add resource not found banner in generic list page, remove deploy button for now and avoid calling find target api if target not installed
- Fix console bug for activating basic section under kubernetes in Asidebar

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Feb 22, 2021
------------
- Rename GenericResourceInnerTable to GenericResourceInnerSection and modularize it into sub component GenericResourceInnerSectionTable.
- Add GenericResourceInnerField component, add logic to show resources either in field mode or list mode, add logic to show create button based on pages api response.
- Discard pages api, integrate resource descriptor api in it's place, read pages from resource descriptor api
- Remove wizard property from resourceToAll, read ui property from resourceDescriptor instead of console-config, remove dependency to resourceToAll form wizard property

Feb 23, 2021
------------
- Integrate new resource descriptor pages changes, fix generic resource inner tables for deatils pages and resource graph.
- Add logic to show Wizard, vue open api form or resource yaml editor components based on the presence of ui.yaml for the resource
- Integrate monaco editor along with all necessary configuration, replace codemirror with monaco-editor in YamlForm component.

Feb 24, 2021
------------
- Update packagees and rollup config to support monaco editor integration and publish v0.1.2.
- Fix error due to presence of 'integer' type in schema in vue-openapi-form.
- Integrate new vue openapi form in console, add resource create functionality to the vue openapi v3 create form

Feb 25, 2021
------------
- Remove default header text, add loader to done button in vue openapi form
- Add fix to the issue where single digit integer/number input is not recorded in vue openapi form

Feb 26, 2021
------------
- Update vue-openapi-form compoent and pass reference model object to show the preview diff in yaml/json tabs
- Integrate vue openapi form in generic resource edit pages
- Fix key value pair first item not showing initially in vue openapi form
- Update yaml form to show preview tab and diff editor in vue openapi form

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

March 1, 2021
-------------
- Fix namespace bug
- Initialize ui jsons for stash initialization step in mongo wizard

March 2, 2021
-------------
- Platform engineering demo meeting
- Add ui element to take prePopulate database and data source as input
- Add ui json to show script related inputs

March 3, 2021
-------------
- Add ui jsons to take backend as input for stash backup restore session repository

March 4, 2021
-------------
- Add ui json for runtime settings pod imagePullSecrets and container resources
- Add ui json for runtime settings container nice and ionice
- Add ui json for environment variable in runtimeSettings for stash initialization

March 5, 2021
-------------
- Complete ui, function and language jsons for mongodb wizard intiialization step
- Work with mohin to synchronize vue-openapi-form with design system (Add small and medium size mode)
- Integrate new vue-openapi-from in console

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

March 8, 2021
-------------
- Add mongodb backup config step and initial jsons
- WIP: adding stash backup configuration form

March 9, 2021
-------------
- Complete adding stash backup configuration form
- Work on adding backup blueprint form

March 10, 2021
--------------
- Fix bug in ui-builde when object returned in computed function is not set
- Fix issue regarding blueprint task parameters not updating in annotations when edited or deleted
- Finish adding backup blueprints form
- Add repository backend type local form jsons

March 11, 2021
--------------
- Merge all the ui, language and function jsons and js for mongo db wizard

March 12, 2021
--------------
- Disable upcoming steps, replace v-show with v-if to prevent rendering all the steps

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

March 15, 2021
--------------
- Add dynamic import to all recursive components in UI builder
- Remove compoent/index.js file, remove global component declarations for recursive components from ui builder
- Add dymanic import to all normal components
- Change rollup configuraltion and wrapper to support lazy loading componetns
- Test Performance in console..
- Update ui-wizard mongo editor ui yamls to latest

March 16, 2021
--------------
- Add disablity checker function for labels field in mongo db editor function js
- Navigate to top of the page when clicking next step
- Test ui-builder

March 17, 2021
--------------
- BB launch status review
- Deploy latest console with ui-builder in appscode ninja for testing
- Fix minor bugs

March 18, 2021
--------------
- Start writing mongo db opsrequest jsons for vertical scaling
- Work on fixing bug in ui-builder

March 19, 2021
--------------
- Finish writing mongo db opsrequest jsons for vertical scaling
- Update desing system and ui-builder in console, (PR review and merge)
- Update ui json in ui-wizard

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

March 22, 2021
--------------
- Platform engineering meeting
- Trim current value and valaue before comparign them, prevents a infinite update bug
- Modify ui json to delete paths if not given by user in vertical scaling ops request
- Prevent on click from working on check radio options if it's disabled by function js
- Add disablity checker for ops request options, disable horizontalScaling for standalone database
- Add horizontal scaling form in mongo ops request

March 23, 2021
--------------
- Add volume expansion and restart ops request form
- Add reconfiguration form except pod template field for mongo ops request


March 24, 2021
--------------
- Add pod tamplate ui json to standalone reconfigure form, fix the json to support nested single step form
- Platform engineering velocity meeting

March 25, 2021
--------------
- Complete reconfigure ops request form for mongo db
- Debug ui-builder
- Plan tasks for zoho

March 27, 2021 (WORK DAY)
-------------------------
- Debug nested delete reactivity issue (Find out problem and rewrite some code and logic)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

March 29, 2021
--------------
- Fix user input not reflecting in model if nested, immediately fire modelValue watchers, always emit value in single step form
- Sprint planning

March 30, 2021
--------------
- Invoke modelValue update functions from store update mutation, fixes Model$update from function js is not working after model$delete in ui-builder
- Fix Nested Single step form array is not setting if path does not exist before

March 31, 2021
--------------
- Fix Attribute removing on model value change is not working
- Update ui builder and add ui jsons to switch between reconfiguration type for standalone mongo db
- Complete adding jsons for reconfiguration ops request for mongo db
- Complete adding jsons for tls configuration ops request for mongo db, publish and test
- Fix MongoDB ops request, when navigated from mongo db operations tab, mongodb details api fails

April 1, 2021
-------------
- Reroute to appropriate list page after create, pass namespace as query to show items of that namespace
- Fix namespace select relatd issues, namespace will initially be selected from query and later stored in store and will be selected from store

April 2, 2021
-------------
- Monthly demo
- Next sprint planning
- WOrk on cluster switcher

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

April 5, 2021
-------------
- Platform engineering meeting
- Add dynamic step support in ui-builder

April 6, 2021
-------------
- Add funciton js support to multistepform, generate showSteps from function js, show or hide sidebar step  based on result of function js and model change
- Fix style of and functionality of cluster switcher while in wizard page

April 7, 2021
-------------
- Rename 'all' namespace option in dropdown to 'All Namespace', keep namespace as query while redirecting by clicking sidebar items
- Plan on modularizing ui-builder

April 8, 2021
-------------
- Implement reusable form element and resolve the ui jsons for the module using function js
- Modify module's ui json to read from it's specific language json
- Support module functions, same new functions via store inside module prefix, change module's funciton reference to match our module prefix
- Add support for resolving prefixed function names
- Resolve module's schema refs by appending and later resolving the prefix, initialize the modelValue in single step form mixin whenever elements change

April 9, 2021
-------------
- Work on ui-builder nested structure design planning
- Fix issue with ui-builder list input form item not editing
- Work on modularizing ui-builder

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

April 12, 2021
--------------
- Platform Engineering meeting
- Fix tab list not updating due to resourceDescriptor api not being called in non generic details pages
- Meeting on auditing other kubernetes dashboards

April 13, 2021
--------------
- Meeting on auditing other kubernetes dashboards
- Disable log tab in pod details until nats is integrated, read tabs from pages api, remove tabs from resource-to-all for pods, removing monitoring tab
- Sort events in descending order according to firstTimestamp and lastTimestamp

April 15, 2021
--------------
- Fix credential create link in cluster create flow (#387)
- Sort list items according to name, remove monitorign from services and prometheus from service monitors (#388)
- Fix mongo ops request create function js
- UI review meeting

April 16, 2021
--------------
- Fix recurring api calls happening in wrong pages, setInterVal not clearing (#389)
- fixed wrong reference of discriminator and multiselect background color issue
- Updated ui json for ops request to handle reconfiguration
- Test opsrequests except tls reconfig

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

April 19, 2021
--------------
- Update node version in console
- Platform engineering meeting
- Pass reusable element ctx through components in order to access it in module function context

April 20, 2021
--------------
- Showcase modularizatoin of ui-builder
- Start integrating dataContext in reusable element
- Test mongodb ops request reconfigure tls

April 21, 2021
--------------
- Add dataContext feature, reactively reference data from model, discriminator, previous dataContext. Prevent referencing data from outside of module context
- Test run mongo create wizard and ops request wizard for the demo.

April 22, 2021
--------------
- Final test run mongo create and ops request wizard
- Organize demo meeting notes

April 23, 2021
--------------
- Organize demo meeting notes
- Perform final checks on console and practice demo for mongo create wizard

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Apirl 26, 2021
--------------
- Platform Engineering meeting
- Sprint planning
- Prevent reusable component from accessing and modifying values outside of it's context via getValue, model, commit and watchDependency

April 27, 2021
--------------
- Allow reusable components to modify data of it's parent elements by passing functionCallbacks from it's parent.
- Integrview for front end candidate
- Showcase modularization for ui builder
- Add modularization docs

April 28, 2021
--------------
- Brief Junayed about ui-builder modularization feature
- Research on state of vue 3 and plan on migrating to vue 3

April 29, 2021
--------------
- Fix ubt function, remove split function, pass reusable element texts prefixed if exists in language.json otherwise pass unchanged to ubt, remove  ubt from single step form array user inputs
- Remove this from mongodb function js, add label field in custom service monitor
- Add showSteps mutations in commitWithContext, pass reusable element ctx in single step form array

April 30, 2021
--------------
- Figure out how to optimize user inputs in ui-builder
- Apply optmization to every form elements

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

May 03, 2021
------------
- Sprint planning
- Platform engineering meeting
- Change emit value using setTimeout to setImmediate, otherwise keyvalue elements save button doesnt save last input, also disable all form elements when value is emitting

May 04, 2021
------------
- Try to fix delay while navigating from wizard page sometimes.
- Dev deploy of cluster-ui for testing on other's computers
- Change cluster name to show spec.display name everywhere except breadcrumb
- Download kubeconfig file now named according to cluster name
- Start working on pod log and execs

May 05, 2021
------------
- Add global terminal component
- Add namespace, pod and container selector for global terminal
- Update and add xtermjs, configure xterm.js

May 06, 2021
------------
- Integrate pod log and exec apis in cluster-ui
- Establish nats connection, declare nats connection as global variable to access it accross whole project

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

May 18, 2021
------------
- Get up to speed after Eid
- Integrate pod log and exec apis, work on terminal component
- Syncup with others
- Update gitea to latest master, test po log and exec
- Prevent user from clearing terminal prompt
- Add terminal copy paste support
- Integrate new log exec api with instance_id support, fixes no unsubscribing issue when shellpath is updated

May 19, 2021
------------
- Sprint planning
- Platform engineering meeting
- Use request instead of publish for exec, listen to errors if, stop listening if error occurs
- Note different page structures and components to be generalized in cluster ui project

May 20, 2021
------------
- Desing, plan and restructure cluster-ui layouts
- Refactor sidebar components, add cluster details and settings page views, make sure to load componets dynamically
- Refactor cluster settings views

May 21, 2021
------------
- Add table components, refactor resource list code without pagination
- Add Header components, add resource list header in resource header view, move console config fetching logic to cluster module in store
- Introduce generic button component, add resource create button in header

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

May 24, 2021
------------
- Implement resource create button, integrate self subject acceess review apis
- Add search bar component and searching feature in resource-table
- Refactor pagination component and add it to resource list table

May 25, 2021
------------
- Add resource details header and tabs component
- Add basic table section, add modal
- Add compnent to handle object type field in tables

May 26, 2021
------------
- Introduce new components to handle object and array type values in table
- Integrate scale button and scale button modal
- INtegrate resource inner table contents, add search feature in content tables

May 27, 2021
------------
- Refactor tables to show data loaders and full table loaders
- Add resource inner content and resource target tables, call targets api from resource module, refactor loaders for table

May 28, 2021
------------
- Add feature to alter between basic mode and list mode in resource tables, add logic to show hide create button
- Add pages route component and show resources for specific pages
- Refactor table loader logic, calc table cell width and show/collapse cell data according to cell width

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

May 31, 2021
------------
- Platform engineerign planning meeting
- Sprint planning
- Refactor events table and events api

June 01, 2021
-------------
- Refactor resource graph components and api calls
- Refactoring resource definition page components and apis

June 02, 2021
-------------
- Add resource create route component, handle logic to konw which create component to render, render resource create editor component
- Refactor resouce create wizard and vue openapi form component

June 03, 2021
-------------
- Refactor config and secret datashow components
- Refactoring cluster basics and node details pages

June 04, 2021
-------------
- Refactor cluster basics pages, connect and remove cluster modals and buttons and node tables along with timeline content
- Add timeline card to resource details pages

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

June 07, 2021
-------------
- Refactored modal compnent, add suport for escape key modal hide, add generic modal component, use vue-portal to teleport modals to desired place
- Refactor node details pages, add nodeDetails api which overrides the resource details api in case of nodes
- Add logic to prevent store actions from setting store state if route is changed while action is being called

June 08, 2021
-------------
- Attatch recurring api calls to resource list, details, targets and events
- Refactor cluster settings pages
- Refactor cluster import page

June 09, 2021
-------------
- Finish Refactor cluster import page
- Refactor cluster list page
- Start code cleanup

June 10, 2021
-------------
- Reposition the form element components and refactor them
- Remove redundant shared tables, loaders, tags, annotations, buttons, charts etc
- Remove images from public, move it to assets, remove redundant assets
- Add terminals component, breakdown terminal component into several sub compnents, add logic to show hide terminal and expand collapse terminals
- Add logic for terminal tabs, adding terminals instances and set active terminal instance

June 11, 2021
-------------
- Add terminal select boxes, add logic to select namespace, pods and containers
- Integrate logging termnal along with api calls
- integrate exec terminal along wiht it's funcitonality, change document margin depending on terminals height

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

June 14, 2021
-------------
- Sprint planning for sprint 2 of june 2021
- Platform engineering planning meeting
- Add Resizing feature in terminals component

June 15, 2021
-------------
- Finalize functionality in terminal components
- Fix cluster list page error, user name missing, read user name from route, if not present of equal to 'kubernetes', then read user name from store
- Add pod log and exec buttons in pod list tables, container and init-container list tables
- Fix terminal loadders and messages, fix top bar username and user fullname, remove profile section from user dropdown, fix sidebar loader

June 16, 2021
-------------
- Stop nats listener when terminal is closed or terminals component is destroyed
- Add resource edit wizard and edit routes, reroute to edit page when edit button is clicked, Add empty table info when table is emtpy
- Fix minor bugs, fix routing to corrent create and edit page wizards for specific resources
- Fix vue dev tools warnings, removed route name from route that has default route child, remove router-link tag prop, use v-slot instead

June 17, 2021
-------------
- Prevent recurring api calls when one api call returns error once
- Fix recurring api calls not stopping even after compnent is destroyed, attach recurring api calls before making actual calls
- Move all the reusable components to design system project and publish them in npm
- Import the reusable components from new design system repo in cluster-ui
- Fix bugs, update design system, update ui-builder in cluster-ui

June 18, 2021
-------------
- Add scroll to top functionality when clicking prevoius button or change active step, also add it when going to actual form from options form and also preview step
- Update design system to v1.0.2, update ui buidler to v1.0.5, fix some issues in accounts ui
- Release cluster ui and accounts ui in dev

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

June 21, 2021
-------------
- Fix terminal exec funcitonality, give fully fledged terminal experience, don't show clusters that are not connected in cluster switcher
- Add loaders to terminal select boxes
- Test mongo create and ops request create wizard
- Deploy cluster ui and accounts ui to production

June 22, 2021
-------------
- Read vite documentation
- Read vue 3, vue-router 4, vuex 4 documentation
- Initialize kubedb-ui project with vite

June 23, 2021
-------------
- Add vue router 4 to the kubedb-ui project
- Add vuex 4 to the kubedb-ui project
- Add axios to the kubedb-ui project, call user api using axios instance and store user in store

June 24, 2021
-------------
- Integrate vue-i18n in kubedb-ui
- Start coverting ui-builder in vue 3

June 25, 2021
-------------
- Work on migrating ui-builder in vue 3

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

June 28, 2021
-------------
- Sprint planning for sprint-2 june 2021
- Define ui json interface in typescript
- Generate schema and apply intellisence using that schema

June 29, 2021
-------------
- Complete store wizard module typescript conversion
- Complete ui builder component typescript conversion
- Add ui json schema to ui-wizards project and apply intellisence to ui jsons
- Update rollup.config.js to typescript and package compnent

June 30, 2021
-------------
- Fix ui-builder errors in kubedb ui project regarding compnent registration and usage
- Integrate and pass store object and i18n languages from kubedb-ui project to ui-builder component
- Read vee-validate 4.0 docs, (compatible with vue 3)

July 01, 2021
-------------
- Convert multi step form component to vue 3 and typescript
- Rewrite multi step form component using vue 3 options api instead of composition api
- Make rollup plugin bundle typescript syntax

July 02, 2021
-------------
- Complete multistep form typescript conversion
- Convert multistep sidebar items to vue 3 and typescript
- Testing ui builder integration with kubedb ui, fixing error in single-step-form-mixin, getValue method

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

July 05, 2021
--------------
- Fix call stack exceed error for resolve schemas, fix resolve function
- Add form element compnent, add form-element components
- WIP: Converting form element component to typescript

July 07, 2021
--------------
- Fillout the 4 performance appraisal forms
- Complete converting form element component into vue 3 and typescript
- COnvert form-element mixn and data function mixin into vue 3 and typescript

July 08, 2021
-------------
- Convert simple input form element into vue 3 and typescript
- Convert tab select element into vue 3 and typescript
- Update ui-schema for ui json validation (it now accepts option values to be objects)
- Convert simple textarea compnent into tyepscript and vue 3
- Mgrate code editor to vue3 and typescript along with integration of monaco-editor in vue 3
- Migrate simple select box component along with mixins to vue3 and typescript, Integrate vue-multiselect next

July 09, 2021
-------------
- Migrate MultiSelectElement to vue 3 and typescript
- Migrate Anchor element to vue 3 and typescript
- Migrate Checkbox and Radio element to vue 3 and typescript
- Migrate Switch element to vue 3 and typescript

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

July 12, 2021
-------------
- Migrate key value input form to vue 3 and typescript
- Migrate key textarea input form to vue 3 and typescript
- Migrate list input form to vue 3 and typescript

July 13, 2021
-------------
- Migrating single-step-form-array to to vue 3 and tyeppscript

July 14, 2021
-------------
- Migrate single-step-form-array to vue 3 and tyepscript
- Debug ui-builder install issue in accounts-ui
- Start migrating reusable-element to vue 3 and typescript

July 15, 2021
-------------
- Migrating reusable-element component to vue 3 and typescript

July 16, 2021
-------------
- 




[ HOME OFFICE ]





---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

August 08, 2021
---------------
- Add top navigation bar
- Add sidebar along with sidebar items, include first level routes and page components
- Redirect user to login page if user api fails

August 09, 2021
---------------
- Add global create button, global create page, show database selection cards, redirect to database create page, add database create page
- Add header components to all the pages
- Add page transition effects

August 10, 2021
---------------
- update vue to latest release for kubedb ui
- Add vue 3 version of content header, content table, form input and searchbar components in design system
- Update vue 3 input component to fix model value not updating bug
- Add vue 3 version of Table and Pagination components and all their dependent components

August 11, 2021
---------------
- Peform vue3 component  modifications according to usage in kubedb-ui
- Change theme color, use vue verison 3.2, Introduce table components along with loaders, search bars, pagination and modals

August 12, 2021
---------------
- Add dropdown element in vue 3
- Add dropdown show hide animation
- Add database list filter component
- Add database select and cluster select to the filter dropdown

August 13, 2021
---------------
- Add namespace select and environment select in database filter
- Randomize database mock api response
- Give type definitions to database types and database statys types
- Add database filter functionality to the database list table
- Clear namespace when cluster is changed in databse filter selections
- Show database type icon in database table

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

August 16, 2021
---------------
- Show recent database list for all the database overview pages
- Show database statuses as tags, add diffrent modifier classes for different statuses
- Show database environemnt as tags in table and add modifier classes to tags as required

August 17, 2021
---------------
- Add database cluster analytics mock api, and show cluster wise analytics
- Add database cluster analytics cards according to design, show analytics table
- Add cluster analytics cards animation
- Add loader for database cluster analytics

August 18, 2021
---------------
- Mover overview header markup to overview header and header cards components
- Add dotted pagination component, paginate overview header items if length exceeds a limit
- Add Semi doughnut percent chart component

August 19, 2021
---------------
- Integrate ChartJS library and Add percent chart component on cluster analytics
- Set overview header card width according to overview header element width
- Set overvie header card number according to minimum width of the header wrapper
- Add animation to numbers in databae overview header
- Add animation to semi doughnut chart percent value
- Add single database cluster analytics cards component

August 20, 2021
---------------
- Add doughnut percent chart, show single database analytics cards and doughnut percent chart inside
- Add number unit composable to separate number and unit from string
- Integrate mock api to single database cluster analytics, add analytics loader component
- Fix chart percent value not reaching full amountby adding percent as key of the chart component

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

August 23, 2021
---------------
- Mock database overview header api, add loader for overview header
- Add loaders to cluster analytics chart component
- Adding fading animation css

August 24, 2021
---------------
- Write kubedb database descriptor structure
- Integrate mock api for database descriptor along with it's type definitions

August 25, 2021
---------------
- Add vue 3 version of Info Table component
- Integrate database details usage header charts
- Integrate database status component, show database status in details header and database list table
- Add tab component, tab bar in database details pages, add feature to switch between tabs
- Add line percent chart component, show line percent chart instead of doughnut chart in database details header
- Add security context compoent, show database security context in details page

August 26, 2021
---------------
- Add database basic table
- Add database insight mock api, show database insight cards in database basic page
- Add loaders to database details header, basic table and insight cards
- Add overview card and cards component in design system

August 27, 2021
---------------
- Add mock grafana charts using mock api in database details page
- Hanlde password type fields in basic table
- Add loaders to database basic chart component

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

August 30, 2021
---------------
- Platform engineering meeting
- Integrate database nodes list mock api and introduce database node list table

August 31, 2021
---------------
- Add insight cards in database insight page
- Add mock api for top collections and slow queries, show top collections and slow queries table in database insight page

September 01, 2021
------------------
- Add mock api for database insight charts, show database insight charts in database insight page

September 02, 2021
------------------
- Add mock api for database backups basics and backup list, add typings, store modules and composables for database backups
- Show database backup basics and recent backups table in backups page, refactor nodes table, slow querties and top collections table
- Add mock api for database opeartions and show database operations list in operations tab
- Add mock api for database alerts overview and list, show database alert list in alerts page

September 03, 2021
------------------
- Merge database details branch to master
- Add expandable feature in backups list table, add expanding animation

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

September 06, 2021
------------------
- Add expandable feature in backups list and alerts list, add actions in alerts list

September 07, 2021
------------------
- Show global alerts and overview in alerts page

September 08, 2021
------------------
- Add filters to alerts list table for global and database local context
- Add filters to backup list table, show recent backups in global backups page, mock global backups api
- Add cluster cell and database type cell in backups list table and alerts list table

September 09, 2021
------------------
- Refactor database list comopnent, lsit filter component
- Refactor database header columns, list filters and table for databse types
- update design system, refactor cluster cell and databse type cell

September 10, 2021
------------------
- Refactor nodes list, queries, collections and operations table
- Refactor alert dropdown actions
- Refactor database overview, add database overview to store module
- FIx typescript errors in database cluster analytics, overview headers cads

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

September 15, 2021
------------------
- Remove vue-tsc validtion from build command, it caused weird errors

September 16, 2021
------------------
- Add sortability in database list table
- Update design system to have sortables tables with fixed issues

September 17, 2021
------------------
- Add theming capability

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

September 20, 2021
------------------
- Add ability to change accent color and font color in design system website
- Use css varaibles for primary color, font color and background color in design system

September 21, 2021
------------------
- Add theming support to kubedbui
- Update table cell value text color to hsl, fix typo in color varaiable name
- Fix CI error, replace the changed variable name accross whole project

September 22, 2021
------------------
- Use overview headercards instead of overview cards in database insights, fix some css issues
- Make nodes table rows linkable, add node details page

September 23, 2021
------------------
- Integrate node descriptor api, along with typees, composables and store modules
- Integrate node details and charts mock api, along with their composables, typings and store module
- Show node details header and node insight headers in node details page

September 24, 2021
------------------
- Show node details overview charts in node details page

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

September 27, 2021
------------------
- Platform engineering planning meeting
- Deploy KubeDB UI in dev cluster
- Start working on accounts ui user management settings

September 28, 2021
------------------
- Write database connection demo nodejs code for MongoDB and Elasticsearch

September 29, 2021
------------------
- Write database connection demo nojdejs code for Postgres, Mysql, Mariadb and Redis

September 30, 2021
------------------
- Write nodejs code to connect to a mongodb database with ssl enabled
- Write doc with instruction to run mongodb nodejs client code

October 01, 2021
----------------
- Write doc with instruction to run elasticsearch, redis, mariadb, mysql and postgres nodejs client code

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

October 04, 2021
----------------
- Push kubedb nodejs client samples to kubedb organization
- Start working on grafana graph generator plugin

October 05, 2021
----------------
- Explore grafana dashboard for v7.5 and v8, explore json structure.
- Explore AssemblyScript

October 06, 2021
----------------
- Setup nodejs typescript project for grafana json generator tool
- Explore different approaches towards building the generator tool
- Explore node-jq library

October 07, 2021
----------------
- Start writing grafana graph dashboard json generator tool

October 08, 2021
----------------
- Start writing typescript types for grafana dashboard object

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

October 11, 2021
----------------
- Platform engineering meeting
- Generate types for grafana dashboard v8
- Compeare between generated types for v8 and v7 dashboard

October 12, 2021
----------------
- Write inputs class and dashobard class, write inputs constructor, generate dashboard json with inputs property
- Write other dashboard basic properties in typescript classes, generate json based on version.

October 13, 2021
----------------
- Write class for templating and generate templating for grafana dashboard json
- Start writing typescript class for panels

October 14, 2021
----------------
- WIP: Writing class for general info row type panel

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

October 18, 2021
----------------
- Write class for row panel
- Understand properties of stat type panel

October 19, 2021
----------------
- Add typescript class for Stat type panel Options
- Add typescript class for Stat type panel Target

October 20, 2021
----------------
- Complete typescript class for Stat type panel
- WIP: Writing class for version stat panel

October 21, 2021
----------------
- Complete writing class for version stat panel
- Construct postgres dashboard json with version stat panel
- Give demo and discuss about changes in grafana json generator

October 22, 2021
----------------
- Work on grafana json generator
- Work on a new approach

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

October 25, 2021
----------------
- Platform engineering planning
- Try to implement convert function as class method for Input class in typescript
- Debugging and fixing typescript errors and warnings

October 26, 2021
----------------
- Write typescirpt type for Dashboard that removes the presence of methods from class
- Write convert function for Input class, call convert function from input instances. 
- Write convert function for Require and annotation class, also read initial config from file

October 27, 2021
----------------
- Write convert function for template variables
- WIP: Write convert function for panels

October 28, 2021
----------------
- Writing convert function for panels
- Write convert function for row type panel and stat type panel
- Write typescript type definitions for panels and sub classes

October 29, 2021
----------------
- Demo the grafana dashboard converter tool
- Write convert function for row and stat chart
- Change the convert function of mappings as per meeting decision
- Write convert function for overrides to account for color overrides

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

November 01, 2021
-----------------
- KubeDB ui, create flow meeting
- Modularize the input config file, modularize the postgres json input into different panel modules

November 02, 2021
-----------------
- Add function to override the panel target exprs based on the dashboard type
- Writing class for timeseries type panel

November 03, 2021
-----------------
- Write Custom class for field config for non row type panel
- Add more stat panels and one timeseries panel to postgres dashboard
- Write Custom class for field config for non row type panel

November 04, 2021
-----------------
- Start writing table panel class
- Research on typescript to conditionally add or remove property from a class structure

November 05, 2021
-----------------
- Refactor the field config and options field for stat and timeseries panels, add timeseries and stat panel sub classes
- Write class for TablePanel along with TableOptions and TableField config fields

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

November 08, 2021
-----------------
- Platform engineering planning meeting
- Write class for various transformations for non row panels

November 09, 2021
-----------------
- Refactor the OmitMethod generic type, add cpu quote table panel
- Add cpu info row panel, cpu usage timeseries panel and memory info row panel in postgres dashboard

November 10, 2021
-----------------
- Add memory quota table panel and memory usage timeseries panel jsons
- Add storage info row, and all storage and disk related panel jsons
- Add network info row, bandwidth receive and transmit timeseries panels

November 11, 2021
-----------------
- Complete postgres dashboard json
- Test the generated dashboard json by loading in in v7 and v8 grafana dashboards and view actual data from panopticon

November 12, 2021
-----------------
- Perform some modifications to panel objects as per requirement
- Test the generated jsons for both versions with real data on real clusters
- Demo the generated dashboards

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

November 15, 2021
-----------------
- Add feature to take source file, version and output dir as command parameters, use semver package to compare between versions

November 16, 2021
-----------------
- Create demo redis database in pg-raft cluster to test grafana dashboard json
- Meeting on KubeDB ui flow

November 17, 2021
-----------------
- Adding dashboard json for redis database overview
- Test the generated redis dashboard for grafana v8
- Write panel json for redis mode stat panel

November 18, 2021
-----------------
- Add redis grafana dashboard typescript object
- remove override for template exprs where it stays the same across databases

November 19, 2021
-----------------
- remove override for template exprs for redis dashboard
- Create grafana-json-converter repo, move grafana type classes to this repo

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

November 22, 2021
-----------------
- Update package json to support npx command and npm publishing
- Publish to npm and test npx command

November 23, 2021
-----------------
- integrade inquirer, select source file, versin and destination folder
- Take root context directory as command parameter for source file

November 24, 2021
-----------------
- Add validation of root path, check if the path exists before starting grafana json converter wizard
- export omitmethod type, import it where required, generate type declaration files

November 25, 2021
-----------------
- Move omit method type declaration inside src folder, revert back to common js module type for this library
- Add separate tsconfig to generate type declarations in a single file, add build and exec scripts in package json

November 26, 2021
-----------------
- Start working on kubedb-ui api integration
- Add clustername to route

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

November 29, 2021
-----------------
- Add username and clustername to routes, add router view files and route navigation guards for proper redirect
- Publish cloud provider icons in cdn.

November 30, 2021
-----------------
- Update design system, update custom.scss, remove lightness function
- Add Cluter switcher in sidebar, switch routes based on selected cluster
- Update design system, remove vue-multiselect dependency from design-system
- Add group, version, resource to routes

December 01, 2021
-----------------
- Review console PR
- Integrating resource summaries api in kubedb-ui

December 02, 2021
-----------------
- Integrate resource summaries api for overview page
- Add cluster database resource summeries to all database pages
- Integrate generic resources api, show database list

December 03, 2021
-----------------
- WIP: integrating resource descriptor api in kubedb ui

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

December 06, 2021
-----------------
- Platform engineering planning meeting
- Integrating descriptor api in kubedb-ui

December 07, 2021
-----------------
- Integrate generic resource descriptor api, comment out database routes, add resource routes and components, descriptor composable, rewrite tabs component
- Add generic field content and generic field table
- Integrate generic resource details api, add resource details typeings and composables, show resource basics table in resource basic page
- Show subtables in resource details page

December 08, 2021
-----------------
- Integrating resource targets api

December 09, 2021
-----------------
- Integrate resource target api, show target resource tables in appropiate tabs

December 10, 2021
-----------------
- 1-1 meeting
- Integrate resource target api, show target resource tables in appropiate tabs

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

December 13, 2021
-----------------
- Remove redundant filters from database filters, move namespace fetch to vuex store, move filtering logic to database list content compoennt

December 14, 2021
-----------------
- Convert database specific routes and components to generic resource routes and components
- Remove overvue store module, api and composable files, move the logic to resource module

December 15, 2021
-----------------
- Update resource table link context, use type of resource to get gvr from table row

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

December 20, 2021
-----------------
- Platform engineering meeting
- Code review

December 21, 2021
-----------------
- Integrate nuxt-bridge, update nuxt.config.js, convert it to typescript, fix linting errors

December 22, 2021
-----------------
- Add typescript support and type declarion file

December 23, 2021
-----------------
- Work on integrating new graph and find api

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

December 27, 2021
-----------------
- Integrate new find api from proxy ui-server
- Use group kind to fetch gvr from reosurceToAll and use gvr to fetch reosurceInfo from resourceToAll

December 28, 2021
-----------------
- Use target resource info from response instead of console-config
- Integrate the new graph api
- Show resource graph with new connections

December 29, 2021
-----------------
- Fix resource graph style
- Remove edge direction
- Highlight root node

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
