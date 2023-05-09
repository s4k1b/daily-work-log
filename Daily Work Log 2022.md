January 03, 2022
----------------
- Platform engineering planning meeting
- Kubedb-ui descriptor update meeting

January 04, 2022
----------------
- Work on integrating tooltip to resource graph
- Analyze the example given in the dagre-d3 library and try to implement it in vue

January 05, 2022
----------------
- Add tooltip feature to resource graph
- Show tooltip on hover, use v-tooltip library, use vue extend feature

January 06, 2022
----------------
- Add style to resource graph tooltip
- Add event listener to graph nodes to go to resource basic page when clicked
- Update design system for resource graph

January 07. 2022
----------------
- Update design system
- make sidebar cluster switcher work
- comment out bakcups and alerts routes

-----------------------------------------------------------------------------------------------------------------------------------

January 10, 2022
----------------
- Meeting about new resource layout and outline
- Integrate new cluster ui namespaced console config
- Refactor resource list to accomodate data object in api response

January 11, 2022
----------------
- Integrate new namespaced console config, refactor resource list to accomodate data object
- Call new resource layout api
- Integrate resource layout api response, calculate pages / tabs from new response

January 12, 2022
----------------
- Initialze resource data from resource layout

January 13, 2022
----------------
- Show all the tables with proper columns generated from resource layout at each page
- Integrating render api

January 14, 2022
----------------
- Integrate render api, call render api for self and sub table kind, sync layout call and render api call
- Call render api for Connections, solve loader conflict issue

-----------------------------------------------------------------------------------------------------------------------------------

January 17, 2022
----------------
- Platform engineering meeting
- Reintroduce recurring api call for resource details pages

January 18, 2022
----------------
- Fix minor bugs, show loader when navigating from one resource instance to another resource instance of save gvr
- Add sorting fucntionality based on api response, move common logic from list and resource list component to mixin

January 19, 2022
----------------
- Add resource error card, show error or missing card based on connection render api response
- Fix redundant isMissing in template error

January 20, 2022
----------------
- Fix resource summar and resource overview tables, account for response formate change

January 21, 2022
----------------
- Integrating resource layout and resource render api in store modules

-----------------------------------------------------------------------------------------------------------------------------------

January 26, 2022
----------------
- Adding store mutations and actions for resource layout and render api

January 27, 2022
----------------
- Adding resource composable for layout and render apis, refactor resource details page

January 28, 2022
----------------
- Added header columsn and tab bar columns with actual data in resource details page, now adding page info, insight and blocks to pages

-----------------------------------------------------------------------------------------------------------------------------------

January 31, 2022
----------------
- Use same route component for  both basic and other pages, show info table if resource info exists
- Remove callbacks from store module and use fetchedOnce to stop loading data once loaded
- Show resource insight in pages where available

February 01, 2022
-----------------
- Platform engineering meeting
- Continue integrating layout and render api in kubedb-ui

February 02, 2022
-----------------
- Review and Merge cluster-ui PR

February 03, 2022
-----------------
- Add sortability in list tables

February 06, 2022
-----------------
- Add fixed with to resource-map format fields in header, use generic cell for generic list tables
- Make recurrent api call using useIntervalFunc in resource overview, list and details pages

-----------------------------------------------------------------------------------------------------------------------------------

February 07, 2022
-----------------
- Prevent updating vuex state for resource summery and list if the resource does not correspond with the current url

February 08, 2022
-----------------
- Perform code clean up, remove unneccessary routes, files and links
- Fix minor bug regarding loader in resource details page, loader vanishes when tab is changed, then data is shown

February 09, 2022
-----------------
- Integrating rendermenu api

February 10, 2022
-----------------
- WIP: Rendering user accordion menu in sidebar, fixing dropdown issue
- Added sidebar item with dropdown component for vue 3 in design system

February 11, 2022
-----------------
- Add overview item under section if section has path, add routes for overview and handle api calls

-----------------------------------------------------------------------------------------------------------------------------------

February 14, 2022
-----------------
- Remove database type composable dependency
- Update design system with sidebar dropdown item, fix some issues

February 15, 2022
-----------------
- WIP: Integrating gallery type user menu in create pages

February 16, 2022
-----------------
- Integrate gallery menu api, show gallery menu in global create, database create and backups create page
- Show create buttons in sections overview and global navbar

February 17, 2022
-----------------
- Refactor usermenu store module and composables
- Meeting about resource-meta update

February 18, 2022
-----------------
- Add redirect from home page to a section overview page or resource overview page
- Filter out the meta columsn from table

-----------------------------------------------------------------------------------------------------------------------------------

February 22, 2022
-----------------
- Meeting on how to edit and view changes resource-meta yamls
- Edit genericresources resourcetabledefinition yaml

February 23, 2022
-----------------
- Update generic cell to corespond to color, link and icon in cell data
- Release planning to do list
- Update generic resources yaml

-----------------------------------------------------------------------------------------------------------------------------------

February 28, 2022
-----------------
- Update resource summeries yaml

March 1, 2022
-------------
- Update podview table definition
- Update mongodbinsights table definition

March 2, 2022
-------------
- Update sorting in Generic list table, edit reosurce tab bar context, update generic cell to show different types of value
- Update mongo slow queries and top colleciton table
- Update podviews to show role column

March 3, 2022
-------------
- Update generic cell and generic list table link generate function
- Update podviews, genericresources and mongodqueries
- Update podviews, generic reosurces, mongo opesrequest, backup sessions table defnitions

March 4, 2022
-------------
- Solve previous data not clearing issue in resource details page
- Add default overview menu icon, update design system to fix warning light color, add resource meta cell to header item in resource details
- Update brackupsoverviews tabel definition

-----------------------------------------------------------------------------------------------------------------------------------

March 07, 2022
--------------
- Resolve redundant api call when switching to pod details page from database details page
- Fixed create button issue in importcluster view

March 08, 2022
--------------
- PR Merge
- Work on accounts ui, refactor components for new table and generic cell component

March 09, 2022
--------------
- Replace accounts ui table-cell with generic-cell and refactor components that uses ac-tables
- PR review and merges
- Discuss about grafana dashboard charts in kubedb-ui

March 10, 2022
--------------
- Show error and missing card for basic and subtable blocks in cluster-ui
- Update dockerfile, use node 14 instead of lts for cluster-ui
- Add status card component, call it in generic field and list content component, replace marketplace with grafana in app drawer in kubedb-ui

March 11, 2022
--------------
- Add create buttons to database overview pages
- Show resource create buttons when necessary

-----------------------------------------------------------------------------------------------------------------------------------

March 14, 2022
--------------
- Fix bugs in resource data loading and change grafana port to 3005
- Test locally and in appscode ninja deployment

March 15, 2022
--------------
- Change reusable component chart version from 0.0.2-alpha.0 to 0.4.0 in ui-wizards
- use chartUrl from resource editor / options instead of hardcoding in resource create wizard in cluster-ui

March 16, 2022
--------------
- Fix redirecting to home page bug in kubedb-ui
- Add status check while importing a cluster, connecting disconnected cluster in cluster-ui

March 17, 2022
--------------
- Debug monaco editor error in appscode.ninja
- Use different library instead of vue-monaco to solve the problem

March 18, 2022
--------------
- Update design system to fix monaco editor error in modals
- Show embedded grafana charts
- Prevent grafana chart url from updating for each recurrent api call from vuex mutation

-----------------------------------------------------------------------------------------------------------------------------------

March 21, 2022
--------------
- Show not exposed when exposed is not used in tab bar, fix bug in global create route, show create button only in opsrequest table
- Update menu, table definitions in resource-meta

March 22, 2022
--------------
- Fix bug in banner.vue component in design system
- Update Editor component to show loading state and error state for monaco editor in design system
- Update cell value, object cell and json show modal to accomodate for object and array type content in design system
- Add spinner in the index.html, this will show while the javascripts are being fetched in kubedb-ui
- Return success color if not exposed, swap position for header app resource request limits, comment out backup section from menu in resource-meta

March 23, 2022
--------------
- Show grafana dashboards table as list of links in kubedb-ui
- Add loader for editor component in modals

March 24, 2022
--------------
- Modify resource-metadata to center align cpu,memory and storage usage table columns along with dashbaord column
- Modify genericresources and show cpu, memory and storage request limit differently

March 25, 2022
--------------
- Show error tooltip only when hovering over error icon
- Update table component, add alert icon if dashboard column returns error, show tooltip
- Update cpu, memory and storage icon in header, update dashbaord link in nodes table in kubedb-ui

-----------------------------------------------------------------------------------------------------------------------------------

March 28, 2022
--------------
- Fix bug regarding menu and other apis when user switches account too fast (before apis for previous user returns)
- Revert header icon size back to 40px
- Recreate and resolve previous data staying issue in kubedb-ui database details pages

March 29, 2022
--------------
- update elastic search reource outline, insight table defintions and schemaoverview and opsrequests
- Fix bug in cluster module, show error field in tab bar context in kubedb-ui

March 30, 2022
--------------
- Write resource outlines and resource table definitions for all other databases

March 31, 2022
--------------
- Add animation to generic cell numeric values, add logic to show hide tab bar context in kubedb-ui
- Update resource outlines and resource tables for elasticsearch, mysql, mariadb, postgres and redis

-----------------------------------------------------------------------------------------------------------------------------------

April 04, 2022
--------------
- Fix table animatable cells not updating when sorting
- Prevent full row reload when recurrent api response returns
- Preview kubedb-ui PR  Add cluster status check in kubebd-ui, show install opscenter core page if cluster status is false

April 05, 2022
--------------
- Add logic to send redirect url when user is redirected to login page in cluster-ui and kubedb-ui
- Update design system and ui-builder to increase the timeout for lazy loaded components in cluster-ui and kubedb-ui

April 06, 2022
--------------
- Research on how to detect if a table has exceeded the screen site (scroller has appeared in table)

April 07, 2022
--------------
- Write MultiInfoTable component, integrate it into kubedb-ui
- Detect when a table has exceeded it's width, show MultiInfoTable in this case

April 08, 2022
--------------
- Update generic list table to show multi info table when list table has scrollbar in kubedb-ui
- update node version to 16 and npm to 8 in kubedb-ui

-----------------------------------------------------------------------------------------------------------------------------------

April 10, 2022
--------------
- Try to setup node version 16 npm 8 environment in cluster-ui

April 11, 2022
--------------
- Platform engineering meeting
- Continue trying to debug issue for cluster-ui ungrading to node 16

April 12, 2022
--------------
- Migrate everthing to latest version and run cluster-ui in node 16 environment without ui-builder

April 13, 2022
--------------
- Migrate everything to latest version and run ui-builder in node 16
- Bundle ui-builder in node 16 environment
- Try to integrate new ui-builder in cluster-ui node 16 environment, debugg errors

April 15, 2022
--------------
- Debug errors when integrating new node 16 ui-builder to cluster-ui

-----------------------------------------------------------------------------------------------------------------------------------

April 17, 2022
--------------
- Debug errors when integrating new node 16 ui-builder to cluster-ui

April 18, 2022
--------------
- Debug and fix errors when integrating new node 16 ui-builder to cluster-ui
- Update packages in kubedb-ui to latest version using npm 8

April 19, 2022
--------------
- Update packages in kubedb-ui to latest npm and node version
- Fix ui-builder vue 3 integration in kubedb-ui
- Start integrating vite to cluster-ui

April 20, 2022
--------------
- Integrate vite to cluster-ui, get dev server running
- Refactor code to support vite system
- Update linting library, rules and code

April 21, 2022
--------------
- Fix linting errors and warnings in cluster-ui
- Update design system and ui builder, integrate them to cluster-ui
- Fix resource graph api call and fix graph library in cluster-ui

April 22, 2022
--------------
- Introduce vue-compat (migration build) to cluster-ui
- Fix errors and warnings

-----------------------------------------------------------------------------------------------------------------------------------

April 25, 2022
--------------
- Fixing errors and warnings in cluster-ui due to migration build

April 26, 2022
--------------
- Fixing errors and upgrading necessary libraries for migration build in cluster-ui

April 27, 2022
--------------
- Fixing errors and warnings regarding migration build in cluster-ui

April 28, 2022
--------------
- Replace vue 2 components from design system with vue 3 components
- Fix breadcrumb compile function issue
- update vue multiselect for vue 3


-----------------------------------------------------EID-UL FITR---------------------------------------------------------------------


May 09, 2022
------------
- Debug v-model warning for migration build in cluster-ui

May 10, 2022
------------
- Migrate components using v-model and child compopnents supporting v-model

May 11, 2022
------------
- Solve watch array and loader not replaced by data issue

May 12, 2022
------------
- REplace set everywhere, replace v2 header with v3 header from design system

May 13, 2022
------------
- Fix resource graph for vue 3 migration build

-----------------------------------------------------------------------------------------------------------------------------------

May 16, 2022
------------
- Convert ResourceDetailsView to composition api, solves  having null in this variable issue
- Use input element in uniqueinputs, update editor,button and form element to vue 3 globally

May 17, 2022
------------
- Update slot name in content-table vue 3 version
- Use ui-builder vue 3 version across full project
- Update ui-builder and pass model-value prop instead of value prop for editor

May 18, 2022
------------
- Add toaster library for vue 3, add composable, replace plugin with composable in some components, add new show error component for toaster
- Replace toaster plugin everywhere with toaster composable

May 19, 2022
------------
- WIP: Migrating vee-validate to latest vue 3 supported version

May 20, 2022
------------
- Fix resource list loading issue when namespace is changed, also add validation in ac multiselect component

-----------------------------------------------------------------------------------------------------------------------------------

May 23, 2022
------------
- Update vuedraggable and fix cluster sidebar settings page
- Replace Validation provider and observer with v field and form across all files

May 24, 2022
------------
- Try to integrate vue 2 version of vue-openapi-form in cluster-ui
- Start migrating vue-openapi-form to vue 3

May 25, 2022
------------
- Update packages for vue 3 and vite, setup vite build and server system, update App, vuex, vueopeapi, object form wrapper and model, validation tabs mixins to vue 3
- Refactor ObjectForm and SimpleInput component into vue 3 syntax
- Refactor Array input, key value input and associated components to vue 3 syntax

May 26, 2022
------------
- Refactor vee validate form error flow and show, error generating function

May 27, 2022
------------
- Use v-slot for form footer to give controls to the client, provide validation function and form state props to the parent
- Test new vue-openapi-form in cluster-ui migration build
- Debug resource graph error in cluster-ui production build

-----------------------------------------------------------------------------------------------------------------------------------

June 2, 2022
------------
- Fix vite build issue in resource graph page
- Integrating vue-openapi-form in cluster-ui

June 3, 2022
------------
- Integrate vue-openapi-form in edit and reslease create pages also
- WIP: Integrate vue network graph library, removing dependency from dagre-d3

-----------------------------------------------------------------------------------------------------------------------------------

June 6, 2022
------------
- Working on integrating vue network graph in cluster-ui migration build

June 7, 2022
------------
- Integrate vue-network-graph, remove d3, dagre-d3 dependency

June 8, 2022
------------
- Test migration build cluster-ui
- Debug Terminal component in cluster-ui

June 9, 2022
------------
- Remove multiple setup function, fix terminal issues

June 10, 2022
-------------
- Refactor configandsecret data component to integrate new resource key value editor component
- Refactor configandsecret data component to integrate new resource key value editor component
- Fix namespace issue when visiting non namespaced resource list, remove namespace from url when visiting resource list with no namespace

-----------------------------------------------------------------------------------------------------------------------------------

June 13, 2022
-------------
- Bump node version of accounts-ui to version 16
- Remove home page from templates and bring it to nuxt
- Add sign up with email in  hero area in accounts ui home page

June 14, 2022
-------------
- Fix style and functionality of signup with bytebuilders in home page
- Trying to add a midddleware for auth check

June 15, 2022
-------------
- Figure out how to read host url in server side
- Start implementing middleware to call user api before entering the home page and redirect appropriately

June 16, 2022
-------------
- Update configm secret data component and fix bug in cluster sidebar settings in cluster-ui migration build
- Remove vue 3 migratiob build dependency, build solely on vue 3, refactor breadcrumb and some comopnents
- Merge cluster-ui vue 3 to master and deploy to appscode ninja

June 17, 2022
-------------
- Remove template pages, remove extended routes logic and go dependency, add auth logic in home page server side
- Write auth middleware file, inclde it in default and user-management layout

-----------------------------------------------------------------------------------------------------------------------------------

June 20, 2022
-------------
- Replace old auth with new server side auth, read api and base domains from environment variables
- Use public runtime config instead of nuxt env

June 21, 2022
-------------
- fix error pages, show 404 if user not found
- Fix various bugs in accounts-ui ssr
- Use runtime config for axios initialization
- Deploy accounts-ui kubedb-ui and cluster-ui latest to appscode ninja

June 22, 2022
-------------
- Add terminals panel, terminal store module and composables, add terminal header buttons
- Add terminal maximize minimize feature
- Add resizing feature in terminals component

June 23, 2022
-------------
- Add tabs adidng and removing feature, tabs changing feature in terminal kubedb-ui

June 24, 2022
-------------
- Add database type and namespace select config in terminal config form
- Add database select option to terminal config form
- Move database list selection logic to composable to reuse in database node select

-----------------------------------------------------------------------------------------------------------------------------------

June 27, 2022
-------------
- Add database node select config, add logic for terminal title
- Add new terminal create banner

June 28, 2022
-------------
- Add nats connection logic, refactor single terminal panel

June 29, 2022
-------------
- Subscribe to nats channel, show logs, add logic to unsubscribe when terminal not active
- Show connecting loader and reconnect button and funcitonality

June 30, 2022
-------------
- Integrate xtermjs in kubedb-ui
- Integrate webGl plugin and Fit addon to xtermjs

July 01, 2022
-------------
- Add log exec button to nodes table
- Modify log icon and add margin bottom to router component when terminal is showing
- Modify terminal style

-----------------------------------------------------------------------------------------------------------------------------------

July 04, 2022
-------------
- Add terminal expanding feature when new instance is added and active instance is changed when collapsed
- Change terminal icon in navbar
- Merge terminal integration PR in kubedb-ui and deploy it

July 05, 2022
-------------
- Update design system, change terminal icon, log exec icon, add webGl renderer to xterm in console
- Add typescript support, add typescript linting rules and fix linting warnings and errors
- Update design system, terminal icon alignment fix in kubedb-ui

July 06, 2022
-------------
- Update resource list view component to composition api and typescript
- fix resource list bug, show error banner if api call returns with error

-----------------------------------------------------------------------------------------------------------------------------------

July 14, 2022
-------------
- Initialize storybook in cluste-rui
- Read storybook docs
- Build long running tast component with storybook

July 15, 2022
-------------
- Discuss with masud regarding long running tasks ui flow
- Initialize long running tasks modal and story

-----------------------------------------------------------------------------------------------------------------------------------

July 18, 2022
-------------
- Add tasks list and logs in long running tast modal along with stories

July 19, 2022
-------------
- Add a simpler mode for long running task modal

July 20, 2022
-------------
- Add notification component and mock notifications

July 21, 2022
-------------
- Add help and switch type button terminal config form
- Add functionality to switch between terminal types

July 22, 2022
-------------
- Add functionality to show hide help panel in terminal, convert markdown to html for help panel

-----------------------------------------------------------------------------------------------------------------------------------

July 25, 2022
-------------
- Add vue-gtag for google analytics in cluster-ui
- Merge terminal help and log/exec switch feature in kubedb-ui

July 26, 2022
-------------
- Add new config in terminal instance for database connect

July 27, 2022
-------------
- Add logic to connect to database
- Handle connect type terminal and change the connection database button position to tab bar

July 28, 2022
-------------
- Add connect button loader and disabling logic, remove edit button from config selections for connect type terminal
- Add conenct context switcher in terminal config and status bar, update select box style

July 29, 2022
-------------
- Adjust to backend channel id expectation for log exec in cluster-ui
- Add functionality to terminal connection context switcher in kubedb-ui
- modify temrinal type switching action, so that id does not need to be changed in kubedb-ui
- Add database connection to database nodes table in kubedb-ui

-----------------------------------------------------------------------------------------------------------------------------------

August 01, 2022
---------------
- deploy kubedb-ui new database connect feature to appscode.ninja
- update package-lock file and ci/release file to support node 16 in deploy-ui
- Migrate build system of deploy-ui to vite

August 02, 2022
---------------
- Perform linting fixes in deploy-ui
- Peform accounts url and api url updates (account and api separation update) in deploy-ui
- Add .vue extension to all the imported vue files in deploy-ui

August 03, 2022
---------------
- Add vue 3, vue 3 specific configurations and vue 3 specific libraries in Deploy UI
- Add defineComponent to every vue file component
- Add defineAsyncComponent to component imports
- Remove components with strpe, replace vue-monaco, update toaster logic and replace Vue with app

August 04, 2022
---------------
- Fix console errors
- Fix AcMultiSelect and AcInputText component

August 05, 2022
---------------
- Remove subscription, card, license part from store, refactor bundle api
- Fix values editor errors, and vue-openapi-form view component

-----------------------------------------------------------------------------------------------------------------------------------

August 08, 2022
---------------
- Replace cluster name with namespace in genericresource column
- Fix bundle api call chart url

August 09, 2022
---------------
- Fix certificate expiration error for local kind cluster
- Fix vue-open-api form styles, integrate new vue-openapi-form (vue 3) version

August 10, 2022
---------------
- Fix vue-openapi-form view, remove subscription, license and card related components and logics

August 11, 2022
---------------
- Work on refactoring final step view in deploy-ui
- Remove get_license api, call bundle to order api

August 12, 2022
---------------
- Fix final step api calls and show commands and scripts

-----------------------------------------------------------------------------------------------------------------------------------

August 15, 2022
---------------
- Platform launch planning meeting
- Merge and publish new deploy-ui in appscode-ninja

August 16, 2022
---------------
- Start integrating new background task api
- Show long running task modal in release create page
- Start integrating nats connection in release create page

August 17, 2022
---------------
- Integrate new release install api with response id for long running task
- Show step wise task modal, show logs

August 18, 2022
---------------
- Add loader for nats connection delay in long running task modal

August 19, 2022
---------------
- Add footer logic and footer success and error buttons and logics for long running tasks
- Complete adding long running task modal to release create flow
- Add long running tasks modal in release rollback

-----------------------------------------------------------------------------------------------------------------------------------

August 22, 2022
---------------
- Add long running tasks modal in release update
- Add long running tasks modal in release uninstall process
- Fix release status filter dropdown and related api call
- Add status and version column in release list table

August 23, 2022
---------------
- Merge release changes to master
- Add long running tasks to managed cluster import

August 24, 2022
---------------
- Add long running tasks to connecting disconnected cluster and some refactoring for managed cluster import
- Add long running tasks to importing public cluster

August 25, 2022
---------------
- Add long running task modal to ui-wizard deploy flow

August 26, 2022
---------------
- Add long running task modal to resource delete process
- Add long running task modal to resource edit page
- Add long running task modal to resource create wizard

-----------------------------------------------------------------------------------------------------------------------------------

August 29, 2022
---------------
- Merge long running task changes for cluster import and database crud to master along with the tests
- Fix general resource delete api url in cluster-ui
- Add long running tasks to resource create page in kubedb-ui

August 30, 2022
---------------
- Add resource delete button in kubebd-ui database details page
- Start integrating long running task modal in delete button

August 31, 2022
---------------
- Add delete resource button and delete resource logic in kubedb-ui
- Publish long running tasks components in design-system

September 01, 2022
------------------
- Move long running tasks components to design system
- Replace local long running tasks components with design system version in cluster-ui and kubedb-ui
- Start integrating notifications api

September 02, 2022
------------------
- Integrate notifications component and nats channel connection

-----------------------------------------------------------------------------------------------------------------------------------

September 05, 2022
------------------
- Add notification component to design system
- Use notification vue 3 components from design system in cluster-ui
- Add notifications feature and components from design-system in kubedb-ui
- Write vue 3 version of notification components in platform-ui

September 06, 2022
------------------
- Add notifications components and nats conneciton feature in accounts-ui
- Refactoring log exec process in cluster-ui

September 07, 2022
------------------
- Integrate new api and nats changes to log exec functionality in cluster-ui

September 08, 2022
------------------
- Integrate new api changes to nats in kubedb-ui and cluster-ui
- Pass theme to long running task component in design-system

September 09, 2022
------------------
- Update build system, discard console logs and debugger in build files in cluster-ui
- Merge design changes by mohin in accounts-ui
- Deploy latest accounts-ui, cluster-ui and kubedb-ui to appscode.ninja

-----------------------------------------------------------------------------------------------------------------------------------

September 12, 2022
------------------
- Platform engineering meeting
- Integrate api in announcement section in platform-ui home page
- Fix server side errors in platform-ui
- Refactor resource graph component, show node details on click, redirect on double click or from tooltip in cluster-ui

September 13, 2022
------------------
- Meeting regarding new tasks
- Start working on integrating recommendations in kubedb-ui

September 14, 2022
------------------
- Add resource icon and reosurce kind to resource nodes in resource graphs
- Meeting on Recommendation table definition and outline

September 15, 2022
------------------
- Declare recommendation table status columns
- Review PRS

September 16, 2022
------------------
- Add recommendation table approve and discard butttons
- Start writing ui-json for approve form

-----------------------------------------------------------------------------------------------------------------------------------

September 19, 2022
------------------
- Added logic to select maintenance window
- Add logic to switch between approval types

September 20, 2022
------------------
- Add logic to show dates array input, update ui-builder to support dates array input

September 21, 2022
------------------
- Add logic to show the recommendation approval form when approve button is clicked inside a modal
- Integrate apis to update recommendation status

September 22, 2022
------------------
- Integrate status update api in recommendation approve flow
- Add recommendation reject apis
- Add comments box in recommendation approve form
- Update ui-builder, teleport ui-builder controls to modal footer for recommendation approve modal

September 23, 2022
------------------
- Fix info center style in standalone single step form in ui-builder
- Update ui-builder, fixes info center in modal for recommendations
- Fix resource update modal logic
- Call appropriate apis for create or edit flow
- Show long running tasks modal

-----------------------------------------------------------------------------------------------------------------------------------

September 26, 2022
------------------
- Merge recommendation feature into master of kubedb-ui
- Start working on contracts in platform-ui

September 28, 2022
------------------
- Add contracts list, add columns and show data

September 29, 2022
------------------
- Add valid user id input field in platform-ui
- Add list input field in platform-ui
- Add contract create form fields and create page in platform-ui

September 30, 2022
------------------
- Integrate contract create api into contract create form
- Handle form data api call for uploading documents in contract

-----------------------------------------------------------------------------------------------------------------------------------

October 04, 2022
------------------
- Add download document button and contract details route
- Add remove and delete api and buttons for contracts
- WIP: updating contract create form or edit functionality

-----------------------------------------------------------------------------------------------------------------------------------

October 10, 2022
------------------
- Integrate contract edit api, reuse contract create form for edit form
- Move contracts store data to contracts module

October 11, 2022
----------------
- Add contracts list in organizaion profile page, fix loader and redirecting issues
- Release latest contacts api integration to appscode.ninja

October 12, 2022
----------------
- Update design-system repo to node-16
- Remove padding in contracts list page in user-management layout
- Integrate contract extend api
- Show download button only to org owner, show org contracts and details to org members
- Remove emails and features columns from contract list page

October 13, 2022
----------------
- Integrate contract audits api, show audits list in contract details page
- Add long running task to monitoring configuration api in cluster-ui

October 14, 2022
----------------
- Fix loading wizard json logic from local in production mode in kubedb-ui
- Test database create and backup configuration flow from kubedb-ui for mariadb database

-----------------------------------------------------------------------------------------------------------------------------------

October 17, 2022
------------------
- Remove marketplace nav-item in platform-ui
- Copy static folder to root in docker image, fixes favicon not present issue in platform-ui
- Test appscode ninja database create, backup and initialize flow

October 18, 2022
----------------
- Ready euronet-test cluster for appscode-ninja demo
- Test database create, backup configuration and restore flow in appscode-ninja and byte-builders
- Give demo to the Euronet team

October 19, 2022
----------------
- Start writing e2e test for contract flow in platform-ui

October 20, 2022
----------------
- Added test for contract list page
- Added test for contract create flow
- WIP: Adding test for contract details flow

October 21, 2022
----------------
- Add test for contract details flow
- Add test for contract edit flow
- Add test to organization contracts flow

-----------------------------------------------------------------------------------------------------------------------------------

October 24, 2022
----------------
- Refactor resource overview page api calls in kubedb-ui
- Introduce backups section and stash resources in sidebar in kubedb-ui

October 25, 2022
----------------
- Add test for sidebar links, verify if ui is redirected right url when sidebar items are clicked
- Call correct apis for backup resources

October 26, 2022
----------------
- Write meta json for kubedb backup configurations layout and table definitions

October 27, 2022
----------------
- Write resource table defintions for all backup type resources in kubedb-ui
- Refactor resource list component to show namespace filters, save resource list api result in store

October 28, 2022
----------------
- Stop calling cluster details on each route change, only call when user or cluster has changed
- Add test for backup configuration overview page
- Add data-testid for corresponding vue3 components in design-system

-----------------------------------------------------------------------------------------------------------------------------------

October 31, 2022
----------------
- Add overview page test for backup sessions, repositories and restore sessions
- Add resource outline blocks for backup configuration
- Add resource block definition for backupconfiguration
- Add target, backup configuration and repository block in backup session outline

November 01, 2022
-----------------
- Add snapshots table definition and show snapshot block in backup session resource block defnitions
- Add resource block definition for respositories and restoresessions
- WIP: Adding test for backup session details page

November 02, 2022
-----------------
- Add details page test for repositories and restore sessions and backup sessions

November 03, 2022
-----------------
- Fix e2e test for authorization and database-overview page
- Run e2e test for whole kubedb-ui

November 04, 2022
-----------------
- Start adding ui.json for repository create ui

-----------------------------------------------------------------------------------------------------------------------------------

November 07, 2022
----------------
- Continue adding ui.json for repository create ui in kubedb-ui

November 08, 2022
-----------------
- Finish adding ui.json for repository create ui in kubedb-ui
- Start adding e2e test for repostiory create flow

November 09, 2022
-----------------
- Add all kinds for e2e test for repository create flow
- Add test for checking if namespace field is disabled when provided in url

November 10, 2022
-----------------
- Create 2 types of menus (kubedb-gallery, kubedb-accordion) for kubedb ui
- Add restoresession struct, generate values schema
- Add restore session values, doc and yaml template

November 11, 2022
-----------------
- Update user menu api to call different menus for gallery and accordion in kubedb-ui
- Add restore session ui json, database select, repository select and snapshot input in ui-wizards
- Add restore session ui repository refresh feature in ui-wizards
- Add restoresession editor options in resource-metadata

-----------------------------------------------------------------------------------------------------------------------------------

November 14, 2022
----------------
- Added storage settings ui in restore session create flow for elasticsearch.
- Start adding runtime config ui in restore session create flow

November 15, 2022
-----------------
- Complete restore session create ui with interimVolumneTemplate and RuntimeSettings forms
- Manually test repository create flow and restore session create flow

November 16, 2022
-----------------
- Add e2e test for restore session create flow
- Open PR in ui-wizards for backup sections

November 17, 2022
-----------------
- Update repository create tests
- Add test for user switching between existing and new secret options
- Refactor resource tab bar context component, bring the control buttons and tab bar context to resource details page
- Remove secret name field from create new secret form in repo create in ui-wizards
- Fix bug in repository create flow, when user switches between existing auth secret to create new in ui-wizards

November 18, 2022
-----------------
- Add database restore button in database details page
- Add restore create flow modal and long running task modal for restore flow
- Add database preselect and disability feature in restore session create ui

-----------------------------------------------------------------------------------------------------------------------------------

November 21, 2022
----------------
- Write e2e test for resource delete button in kubedb-ui
- Platform engineering meeting
- Start working on operations menu

November 22, 2022
-----------------
- Add resource operations menu api, module and composables, add menu button, modal and reosurce wizard modal in kubedb-ui
- Add funcionality for resource wizard modal, handle different flows for self edit, new create and new create without charts in kubedb-ui
- Update mariadb ops request jsons in ui-wizards to support kubedb-ui operations

November 23, 2022
-----------------
- Update restore session create ui and function json for kubedb-ui operations
- Add timing and apply fields to mariadb opsrequest
- Work on operations for elasticsearch

November 24, 2022
-----------------
- Remove memcached from kubedb menus, make repository name in backupoverview table clickable
- Update opsrequest create ui for all database, change updgrade to updateVersion in redis opsrequest

November 25, 2022
-----------------
- Don't disable operations button when datbase is not ready in kubedb-ui
- Remove resource tab bar context click feature, modify create button show logic in blocks in kubedb-ui
- Make long running tasks simpler in kubedb-ui
- Modify database outlines to remove create button from all blocks in resource-meta

-----------------------------------------------------------------------------------------------------------------------------------

November 28, 2022
-----------------
- Update ui-builder for using time-input component in kubedb-ui
- Fix i18n update issue, perform lint fixes in ui-builder
- Add i18n composable in reusable element, remove vscode config from gitingnore in ui-builder
- Add time input element component logic in ui-builder
- Add time input element for timeout section in opsrequests in ui-wizards

November 29, 2022
-----------------
- Integrate resource actions, in resource layout and render api response in kubedb-ui
- Update libraries and perform linting fixes in kubedb-ui
- Fix errors related to renaming operations to actions in kubedb-ui
- Update mariadb editor actions in resource-meta

November 30, 2022
-----------------
- Update ui-builder to latest in kubedb-ui
- Update editor actions for all the kubedb-ui databases in resource-meta
- Add disableTemlpate in database actions where required in resource-meta
- Modify database type functions for mysql and postgres opsrequests in ui-wizards

December 01, 2022
-----------------
- Add global layouts api mock, rearrage cypress fixture files in kubedb-ui
- Ignore namespace change on resource layout and descriptor api call, fixes layout loading issue when namespace is changed before layout api resolves in cluster-ui
- Fix error on contract details page if contract does not exists, redirect to list page in this case in platform-ui
- Fix test error for credential delete e2e test in platform ui

December 02, 2022
-----------------
- Fix cluster menu not setting when redirecting from cluster-status page in kubedb-ui
- WIP: adding proxy sql resource outlines and defintions and connections

-----------------------------------------------------------------------------------------------------------------------------------

December 07, 2022
-----------------
- WIP: work on adding resource-meta files for proxy sql

December 08, 2022
-----------------
- Show N/A if resource usage data does not exist in kubedb-ui
- Add proxysql dashboard in resource dashoboard and pods in resource-meta
- Add proxysql presets and dashboards supports in the kubedb and bytebuilders installer

December 09, 2022
-----------------
- Add actions for proxysql, also add reconfigure action to all the databases in resource-meta
- Add reconfigure opsrequest to the initOpsrequest function in database opsrequests in ui-wizards
- Update opsrequest type function in database edit uis in ui-wizards
- Add apply action feature from route query on details page load in kubedb-ui

-----------------------------------------------------------------------------------------------------------------------------------

December 11, 2022
-----------------
- Add apply action feature from route query on details page load in kubedb-ui
- Fix redirect to list page in cancel button is clicked in resource create wizard in cluster-ui
- Add custom compare function for step idenfiers, direct string compare does not work in ui-builder

December 12, 2022
-----------------
- Work on various issues in ui-builder

December 13, 2022
-----------------
- Work on ui-builder issue

-----------------------------------------------------------------------------------------------------------------------------------

December 19, 2022
-----------------
- Platform engineering meeting
- Work on ui-builder single step form array required issue

December 20, 2022
-----------------
- Ui-builder debugging

December 21, 2022
-----------------
- Fix required field validation for hidden forms in ui-builder
- Fix required field validation for form array in ui-builder

December 22, 2022
-----------------
- PR reviews
- Package ui-builder with latest changes
- Discuss scanner api integration in cluster-ui
- Work on resulting bug in ui-builder

December 23, 2022
-----------------
- Fix required error when whole object is required but part of the object is refered in the ui
- Find out where fields are unneccessarily required in the option schemas

-----------------------------------------------------------------------------------------------------------------------------------

December 26, 2022
-----------------
- Check different options charts for required validation errors
- Plan on cluster report page structure
- Add cluster report route, store module and type in cluster-ui

December 27, 2022
-----------------
- Migrate vuex store to typescript
- Add test for cve report sidebar item and loader
- Create a flow of data for cluster report stats in cluster report header

December 28, 2022
-----------------
- Show reoprt stats in header, add test to verify if stats are shown in cluster-ui
- Add vulnerability table, create data flow for vulnerability table in cluster-ui report page

December 29, 2022
-----------------
- Add vulnerability details component, data flow, store properties and apis in cluster-ui

December 30, 2022
-----------------
- 