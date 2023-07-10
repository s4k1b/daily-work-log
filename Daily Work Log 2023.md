January 02, 2023
----------------
- Fix images table columns and value formats in cluster-ui report page
- Add data flow for image lineages, add types and store data in cluster-ui

January 03, 2023
----------------
- Add image lineage card component and logic to show image lineages chain in cluster ui report page
- WIP: Adding functionality to highlight image from image report when image name is clicked from vulnerability report

January 04, 2023
----------------
- Add feature to scroll and expand image from image report table in cluster ui report page
- Add feature to keep only one row expanded at a time in cluster-ui report page tables

January 05, 2023
----------------
- Replace index.docker.io at the start of image names with empty string in cluster-report tables
- Added request interceptor for axios, adding response interceptor for caching

January 06, 2023
----------------
- Start adding caching logic for render apis

-----------------------------------------------------------------------------------------------------------------------------------

January 09, 2023
----------------
- Added cache control for render apis, convert render apis to get call
- Add cache control to render menu put api

January 10, 2023
----------------
- Add cache control to resource create wizard, create apis and delete api
- Upgrade marketplace ui to node 16

January 11, 2023
----------------
- Update e2e test for rendermenu and render api changes in cluster-ui
- Move caching logic to design-system in cluster-ui
- Update rendermenu and render api calls to get calls with query string, update the tests and design system in kubedb-ui
- Add axios interceptors, modify list and render api calls, so that it performs cache controls in kubedb-ui

January 12, 2023
----------------
- Update caching plugin from design system in cluster-ui
- Convert cluster report apis to get calls with query, also fix collapsible issue in cluster-ui
- Add cache control to resource create, edit and delete apis in kubedb-ui
- Update e2e tests for ctag in kubedb-ui

January 13, 2023
----------------
- Added grafana charts in cluster-report page in cluster-ui
- Adding charts to vulnerabiltiy stats in cluster-ui report page

-----------------------------------------------------------------------------------------------------------------------------------

January 16, 2023
----------------
- Add charts to image report details in cluster-ui
- Add vulnerabiltiy count occurrence table and chart for cluster-report page in cluster-ui

January 17, 2023
----------------
- Add logic to handle zero count or occurrence values in vulnerabilty charts in cluster-ui
- Make vulnerability details section background color dynamic in cluster-ui
- Add table collapse animation, move report chart styles to design-system in cluster-ui

January 18, 2023
----------------
- Add composable for ui theme, change grafana panel theme based on ui theme
- Start working on report request form

January 19, 2023
----------------
- Add scan report filter form, show vulnerability details for vulnerability report in cluster-ui
- Show image lineage in cluster report page for image report in cluster-ui
- Add loader for report vulnerability, update design system

January 20, 2023
----------------
- Update ci file for installing cypress dependencies
- Clear old connection error for long running tasks, fixes but if error occurrs
- Fix api call for app report
- Add cve reports to app security pages

-----------------------------------------------------------------------------------------------------------------------------------

January 23, 2023
----------------
- Sketch sample yaml to incorporate sections inside pages in resource outlines
- Start working on new project named ui-modules to house and develop various ui modules for bytebuilders platform

January 24, 2023
----------------
- Add user, cluster and resource list page layouts and componetns in ui-modules
- Add resource details views and route components in ui-modules
- Add axios, domain and caching plugin in ui-modules
- Add store, api, and type modules for cve reports in ui-modules

January 25, 2023
----------------
- Add cve report vue comopnents in ui-modules
- Install and intergrate the cve report moduels from ui-modules to cluster-ui
- Add cluster api calls, store module and typings, add further store functions to write easily writable store actions in ui-modules

January 26, 2023
----------------
- Refactor store and cluster module code for better type definitions ui modules

January 27, 2023
----------------
- Add usermenu module, composables and typings in ui-modules
- Further refactoring ui-modules store components

-----------------------------------------------------------------------------------------------------------------------------------

January 30, 2023
----------------
- WIP: Type refactoring for cve reports and other store modues in ui-modules

January 31, 2023
----------------
- Refactor Cve report components with store util functions in ui-modules
- Add more cluster api calls and cluster store module actions in ui-modules
- Refactor and add more properties to cluster composable

February 01, 2023
-----------------
- Refactor cluster type and list api call and namespace type and api calls in ui-modules
- Add function to get the status of cluster status by cluster name in cluster composable in ui-modules
- Add nodes list and fetching status in cluster composables and fetching action in cluster composables in ui-modules
- Integrate cve report modules from ui-modules in cluster-ui
- WIP: Replacing old cluster module with new module and composable from ui-modules in cluster-ui

February 02, 2023
-----------------
- Replacing old cluster module with new module from ui-modules in cluster-ui
- Add function to get and set active namespace in cluster composable in ui-modules

February 03, 2023
-----------------
- Replace old existing cluster module with ui-module's cluster-module in cluster-ui
- Update cluster resources setting logic in ui-modules
- Add form field components and icons in ui-modules
- Refactor cve report logic in ui-modules

-----------------------------------------------------------------------------------------------------------------------------------

February 06, 2023
----------------
- Update ui-modules and fix some bugs in resource details view in cluster-ui
- Replace old usermenu and cluster modules with new ones from ui-modules in kubedb-ui
- Perform various changes as per requirement from kubedb-ui and cluster-ui in ui-modules

February 07, 2023
----------------
- Update ui-modules, modifies image lineage links in cluster-ui and kubedb-ui
- Add cve report for databases, integrate cve report module from ui-modules in kubedb-ui
- Modify Image lineage link, handle based on ui domain in ui-modules

February 08, 2023
-----------------
- Replace old resource info mixin with resource compsable, updte vite to v3 in cluster-ui
- serialize query params in axios request interceptor in ui-modules

February 09, 2023
-----------------
- Optimize crypto-js and axios module, remove storybook in cluster-ui and kubedb-ui
- Merge ui-modules changes to master for cluster-ui and kubedb-ui

February 10, 2023
-----------------
- Start integrating resource module in ui-modules
- Add universal sidebar component in ui-modules

-----------------------------------------------------------------------------------------------------------------------------------

February 13, 2023
----------------
- Add universal sidebar component in ui-modules
- Initialize resource modules, apis and composables in ui-modules

February 14, 2023
-----------------
- Platform meeting
- Integrate resource layout api call and store variables in ui-modules

February 16, 2023
-----------------
- Add resource view composable, add reosurce layout api calls, and store variables in ui-modules

February 17, 2023
-----------------
- Add resource details sidebar component and logic in ui-modules
- Integrate resource render api, handle api response and related store states and types
- Add resource render page and block, bring generic tables and cels from kubedb-ui to ui-modules

-----------------------------------------------------------------------------------------------------------------------------------

February 20, 2023
----------------
- WIP: Adding resource render response store functionality in modules

February 22, 2023
-----------------
- Integrate resource render api response, add store functionality in modules and show rendered tables
- Refactor generic list and field tables and add status block, wip: adding recurrent api calls via recursion

February 23, 2023
-----------------
- Inplement recurring api call composable in ui-modules
- WIP: Adding grafana charts and other block components in ui-modules

February 24, 2023
-----------------
- Handle internal resource table action buttons and block action buttons via slots in ui-modules

-----------------------------------------------------------------------------------------------------------------------------------

February 27, 2023
----------------
- Integrate resource list api and composables in ui-modules

February 28, 2023
-----------------
- Add rest of the resource details page apis and store actions in ui-modules
- Start integrating new ui-modules logic in cluster-ui

March 01, 2023
--------------
- Update generic list table to force row links and handle labels colum in ui-modules
- add feature to add /kubernetes based on route path in row and row cell links in ui-modules
- Integrate resource list functionality from ui-modules in cluster-ui

March 02, 2023
--------------
- Add custom resource details pages and integrate ui-modules in events, graph and definition page in cluste-rui
- Integrate ui-modules in resource defintion content and patch button in cluster-ui

March 03, 2023
--------------
- Integrate ui-modules in resource create and edit flow in cluster-ui

-----------------------------------------------------------------------------------------------------------------------------------

March 06, 2023
----------------
- Make namespace optional in handle cache yaml function in ui-modules
- Calculate if block rows are actionable in resource block component in ui-modules
- Integrate ui-modules in resource delete flow in cluster-ui
- Integrate ui-modules in resource scale button in cluster-ui

March 07, 2023
--------------
- Call cve report apis in reosurce details view composable, add slots in resource render page and Fix typings for resource definition in ui-modules
- Add resource create button in resource page view in cluster-ui

March 08, 2023
--------------
- Fix error in Cluster sidebar for release pages in ui-modules
- Integrate ui-modules in config data component, resource apply button and create editor in cluster-ui
- Fix release pages and store components, remove resource store module and composable in cluster-ui

March 09, 2023
--------------
- Remove resource components, replace with generic comopnent from ui-modules in cluster-ui
- Complete integration for resource modules from ui-modules in cluster-ui
- Fix bug related to cluster sidebar route group and version not being present for cluster settings page in ui-modules

March 10, 2023
--------------
- Remove cluster main sidebar component, use comopnent from ui-modules
- Fixing e2e tests after ui-modules integration

-----------------------------------------------------------------------------------------------------------------------------------

March 13, 2023
----------------
- Fix e2e test errors in cluster-ui
- Update ui-modules and fix vite build issue in cluster-ui
- Handle undefined image stats in image report table in ui-modules
- Move utility functions from resource composables to plugins in ui-modules

March 14, 2023
--------------
- Replace sidebar with cluster sidebar from ui-modules in kubedb-ui
- Integrate ui-modules in datastore overview page in kubedb-ui
- Handle sections type resources in sidebar overview options in ui-modules
- Fix resource list action for kubedb datastore section in kubedb-ui

March 15, 2023
--------------
- Switching between reosurce list pages clears namespace in cluster-ui
- Integrate ui-modules in resource overview page, Integrate ui-modules in resource view in kubedb-ui
- Fix recurring api calls for kubedb-ui, resource list pages with label selector in ui-modules
- Handle route change between datastore sections and resource list in ui-modules

March 16,2023
-------------
- Update resource render block composable to handle header and tabBar blocks in ui-modules
- Integrate ui-modules in resource details header and tabbar context in kubedb-ui
- Integrate resource render page from ui-modules in kubedb-ui

March 17, 2023
--------------
- INtegrate ui-modules resource module in resource connect and delete button in kubedb-ui
- Integrate resource module in action button and action modal in kubedb-ui
- Integrate ui-modules resource module in log exec, recommendation, resource create and details page in kubedb-ui

-----------------------------------------------------------------------------------------------------------------------------------

March 20, 2023
----------------
- Refactor resource wizard modal, create pages and overview headers in kubedb-ui

March 21, 2023
--------------
- Fix nodes page and stash resource details pages bug
- Remove icons from generic cell in ui-modules

March 23, 2023
--------------
- Add suspense and loader to details components in kubedb-ui
- Merge ui-modules resource branch to master, along with cluster import changes

March 24, 2023
--------------
- Return functions to resource view and resource details view to be called from the vue components in ui-modules
- Start merging cluster create/imoprt flow with master and ui-modules implementation

-----------------------------------------------------------------------------------------------------------------------------------

March 27, 2023
----------------
- Platform engineering meeting
- Merge cluster-ui import cluster and ui-modules branches

March 28, 2023
--------------
- Merge import-cluster and ui-modules changes to cluster-ui
- Merge import-cluster and ui-modules changes to kubedb-ui

March 29, 2023
--------------
- Minor bug fixes and PR review in cluster-ui
- Look into kubedb-ui navigation speed issue after ui-modules integration

March 30, 2023
--------------
- Look into kubedb-ui navigation speed issue after ui-modules integration

March 31, 2023
--------------
- Fix navigation slowness, update ui-modules in kubedb-ui
- Review and merge PRs to fix cluster-ui tests
- Start working on resource details page, tabs and sections changes

-----------------------------------------------------------------------------------------------------------------------------------

April 03, 2023
----------------
- Refactor resource details page modules, support sectioned blocks and custom blocks, custom cve report block in ui-modules
- Support section pages in resource details sidebar in ui-modules

April 04, 2023
--------------
- Support sections in resource details outlines in ui-modules
- Add option to force connected resource link in resource details page in ui-modules (needed for cluster-ui)
- Give brief introduction to resource-meta to Riyad & Arnob
- Update cluster-ui tests for changed resource layout (sections integration)

April 05, 2023
--------------
- Add security sections for databases default layout in resource-metadata
- Move access control block to rbac folder in resource block outlines

April 06, 2023
--------------
-  Add security sections to resource details pages, add security overview page in cluster menu outline in resource-meta
- PR review and merge

April 07, 2023
--------------
- Add kafka options files in ui-wizards
- Add kafka editor and options charts in resource-metadata

-----------------------------------------------------------------------------------------------------------------------------------

April 10, 2023
----------------
- Platform engineering meeting
- WIP: Adding editor charts for kafka

April 11, 2023
--------------
- Update kafka options schema, create-ui and language json
- Add kafka editor chart files
- Add kafka editor create-ui files

April 12, 2023
--------------
- Modify kafka editor and options ui as per review in ui-wizards
- Add kafka edit ui in ui-wizards

April 13, 2023
--------------
- Remove enableSSL from values file, SSL will be enabled from editor create-ui TLS step in kafka wizard
- Add resource outline, block defintion, table defintion and connections for kafka in resource-metadata
- Update kafka custom yaml in ui-samples
- Add generate command for kafka in lib-app

-----------------------------------------------------------------------------------------------------------------------------------

April 17, 2023
----------------
- Add kafka option to kubedb menu, add icons of kafka and redissentinels in resource metadata
- Add kafka resource outlines, grafana dashboards files and podview table for kubedb-ui in resource-metadata

April 18, 2023
--------------
- Add kafka outline for kubedb-ui, add missing icons to resources in resource-metadata
- Try to add kafka to generic resources and resource summaries

-----------------------------------------------------------------------------------------------------------------------------------

April 26, 2023
----------------
- Pass source ref instead of chart url to ui-builder in cluster-ui
- Replace chart url with sourceRef in ui-builder and build for production
- Replace chart url with sourceRef for chart api calls in functions js in ui-wizards

April 27, 2023
----------------
- Integrate chart url fix changes in kubedb-ui
- Test and report errors regarding the chart url fix

April 28, 2023
--------------
- Chart url fix, replace chart url with source ref, update ui-builder and ui-modules in cluster-ui
- Replace chart url with sourceRef in kubedb-ui

-----------------------------------------------------------------------------------------------------------------------------------

May 02, 2023
----------------
- Meeting regarding helm chart issue
- Guide the new hires
- Add actions for kafka kubedb-ui in resource-metadata

May 03, 2023
------------
- Add status colors to phase columns for cluster-ui databases in resource-metadata
- Adding e2e tests for kafka create ui in kubedb-ui

May 04, 2023
------------
- Add e2e tests for kafka create ui in kubedb-ui
- Start working on Policy report

May 05, 2023
------------
- Change resource delete wizard api url and query params in ui-modules
- Debug and test b3 resource-meta branch

-----------------------------------------------------------------------------------------------------------------------------------

May 08, 2023
------------
- Platform Engineering Meeting
- Add policy report store, type and composables, add policy report api call and call api in resource details page (ui-modules)

May 09, 2023
------------
- Show policy constraint list in policy report block in ui-modules

May 10, 2023
------------
- Add policy details in policy report block in ui-modules
- Add policy violations

May 11, 2023
------------
- Setup workstation
- Import cluster test
- Work on Policy report ui

May 12, 2023
------------
- Add tooltips for violation list in ui-modules
- Add gatekeeper cluster level and namespace level report ui in ui-modules

-----------------------------------------------------------------------------------------------------------------------------------

May 16, 2023
------------
- Add banner to show no constraints if the constraint list is empty in ui-modules
- Add pagination feature to violation list and fix maximum height to constraint list in ui-modules

May 17, 2023
------------
- Move policy report logic to composable in ui-modules
- Integrate gatekeeper report components in cluster-ui

May 18, 2023
------------
- Update complete usermenu api call to generate complete cluster resources for both kubedb ui and cluster ui in ui-modules
- Fixing bug in implementation of policy report in kubedb-ui

May 19, 2023
------------
- Fix bug in implementation of policy report in kubedb-ui
- Update cve report test in cluster-ui

-----------------------------------------------------------------------------------------------------------------------------------

May 22, 2023
------------
- Platform meeting
- Test and report bug on cluster-ui import and database create flow
- Upgrade ui-builder to node 18

May 23, 2023
------------
- Migrate ui-modules, cluster-ui and kubedb-ui to node 18
- WIP: Migrate platform-ui to node 18

May 24, 2023
------------
- Migrate platform-ui, selfhost-ui, learn-ui to node 18
- Meeting about future work
- Scaffold new vue project for billing ui

May 25, 2023
------------
- Add linting, styling and vscode settings in billing-ui
- Get stylelint working, add our design system in billing-ui

May 26, 2023
------------
- Add topbar and sidebar to billing ui, add routes and vuex
- Fix grafana dashboard theme and cve report api calls in kubedb-ui and cluster-ui

-----------------------------------------------------------------------------------------------------------------------------------

May 29, 2023
------------
- WIP: Adding user authentication in billing-ui

May 30, 2023
------------
- Add user authentication and user dropdown in navbar in billing ui
- Update design system vue 3 branch
- Report various issues to Masud and Arnob

May 31, 2023
------------
- Add sidebar option highlight on route change in billing-ui
- Handover billing ui depelopment over to Nihal
- Review everyone's work
- Setup console-demo cluster for local ui development

June 01, 2023
-------------
- Setup console-demo cluster again for local ui developement with the help of masud
- Review everyone's work
- Research on serving multiple vue apps under the same domain

June 02, 2023
-------------
- Finish research on serving multiple vue apps under the same domain
- Start reading vitepress documentation

-----------------------------------------------------------------------------------------------------------------------------------

June 05, 2023
------------
- Research on vitepress
- Platform Engineering Meeting
- Review everyone's work

June 06, 2023
-------------
- Scaffold bytebuilders docs project using vitepress.
- Review everyone's work

June 08, 2023
-------------
- Add typescript and linting support to docs project
- Review everyone's work and assist theme

June 09, 2023
-------------
- Add page links and page metas to docs website
- Move docs to src folder
- WIP: Debug typescript error from ui-modules

-----------------------------------------------------------------------------------------------------------------------------------

June 13, 2023
------------
- Move components folder to vitepress theme folder
- Add useFetch custom for api calls, also add pinia

June 14, 2023
-------------
- Add user store, read user store from docs
- Add user dropdown, login logout feature

June 15, 2023
-------------
- Add i18n support and language switching mechanism to docs ui

-----------------------------------------------------------------------------------------------------------------------------------

June 19, 2023
------------
- Platform engineering meeting
- Review everyone's work
- Review vue vitepress docs implementation

June 20, 2023
-------------
- WIP: Working on integrating docs sidebar
- Work with Nihal and Riyad separately to assist in solving problems
- Review work

June 21, 2023
-------------
- Add sidebar config, show sidebar based on config
- Review work and bug fixes

June 22, 2023
-------------
- And language switching support to sidebar links in docs
- Fix sidebar bugs and typings fix in docs

June 23, 2023
-------------
- Add document outline as right sidebar

-----------------------------------------------------------------------------------------------------------------------------------

June 26, 2023
-------------
- WIP: Adding functionality to highlight currently active outline in docs

June 27, 2023
-------------
- Add document outline hightlight feature based on scroll position
- WIP: Research on search feature

-----------------------------------------------------------------------------------------------------------------------------------

July 03, 2023
-------------
- Platform engineering meeting
- Read meilisearch docs and test implementation
- Review kubedb website docs meilisearch implementation
- Review test pr in cluster ui

July 04, 2023
-------------
- Add meilisearch configuration in theme, integrate meilisearch api calls and search bar

July 05, 2023
-------------
- Add footer navigation for docs pages in docs-ui
- Meeting abou opcenter ui and JMAP

July 06, 2023
-------------
- Start reading JMAP client docs

July 07, 2023
-------------
- Test and report issues for elasticsearch, mysql, redis create and details pages
- JMAP client docs

-----------------------------------------------------------------------------------------------------------------------------------

July 10, 2023
-------------
-


