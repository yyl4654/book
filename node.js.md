# Node.js

### Overview <a href="#overview" id="overview"></a>

GitBook provides an official Typescript/Javascript client for the HTTP API. This client can be used in a browser or Node.js environment.

### Installation <a href="#installation" id="installation"></a>

You can install the GitBook Node.js library through `npm`.

### Usage <a href="#usage" id="usage"></a>

**General usage:**

```
import { GitBookAPI } from '@gitbook/api';

const client = new GitBookAPI({
  authToken: <your_access_token>
});
```

**Usage with Node.js**

When using the `@gitbook/api` module with Node.js < v18, you should pass a custom `fetch` function.

You can install one using the [`node-fetch`](https://github.com/node-fetch/node-fetch) module.

```
import { GitBookAPI } from '@gitbook/api';
import fetch from 'node-fetch';

const client = new GitBookAPI({
  customFetch: fetch
});
```

### Reference <a href="#reference" id="reference"></a>

#### Search <a href="#search" id="search"></a>

The following methods can be found on the `client.search` object.

| Method            |
| ----------------- |
| `searchContent()` |
| `askQuery()`      |

#### User <a href="#user" id="user"></a>

The following methods can be found on the `client.user` object.

| Method                             |
| ---------------------------------- |
| `getAuthenticatedUser()`           |
| `listSpacesForAuthenticatedUser()` |

#### Users <a href="#users" id="users"></a>

The following methods can be found on the `client.users` object.

#### Spaces <a href="#spaces" id="spaces"></a>

The following methods can be found on the `client.spaces` object.

| Method                                   |
| ---------------------------------------- |
| `getSpaceById()`                         |
| `searchSpaceContent()`                   |
| `askQueryInSpace()`                      |
| `importGitRepository()`                  |
| `exportToGitRepository()`                |
| `getContentAnalyticsForSpaceById()`      |
| `getSearchAnalyticsForSpaceById()`       |
| `getTrafficAnalyticsForSpaceById()`      |
| `trackViewInSpaceById()`                 |
| `getCurrentRevision()`                   |
| `importContent()`                        |
| `listFiles()`                            |
| `getPageById()`                          |
| `importContentInPageById()`              |
| `getPageByPath()`                        |
| `createChangeRequest()`                  |
| `mergeChangeRequest()`                   |
| `updateChangeRequest()`                  |
| `getRevisionOfChangeRequestById()`       |
| `importContentInChangeRequest()`         |
| `listFilesInChangeRequestById()`         |
| `getPageInChangeRequestById()`           |
| `importContentInChangeRequestPageById()` |
| `getPageInChangeRequestByPath()`         |
| `getRevisionById()`                      |
| `listFilesInRevisionById()`              |
| `getPageInRevisionById()`                |
| `getPageInRevisionByPath()`              |
| `listPermissionsAggregateInSpace()`      |

#### Collections <a href="#collections" id="collections"></a>

The following methods can be found on the `client.collections` object.

| Method                                   |   |   |
| ---------------------------------------- | - | - |
| `getCollectionById()`                    |   |   |
| `listSpacesInCollectionById()`           |   |   |
| `listPermissionsAggregateInCollection()` |   |   |

#### Integrations <a href="#integrations" id="integrations"></a>

The following methods can be found on the `client.integrations` object.

| Method                                 |
| -------------------------------------- |
| `listIntegrations()`                   |
| `getIntegrationByName()`               |
| `publishIntegration()`                 |
| `unpublishIntegration()`               |
| `listIntegrationInstallations()`       |
| `listIntegrationSpaceInstallations()`  |
| `renderIntegrationUiWithGet()`         |
| `renderIntegrationUiWithPost()`        |
| `updateIntegrationInstallation()`      |
| `createIntegrationInstallationToken()` |
| `updateIntegrationSpaceInstallation()` |

#### Orgs <a href="#orgs" id="orgs"></a>

The following methods can be found on the `client.orgs` object.

| Method                                    |
| ----------------------------------------- |
| `listOrganizationsForAuthenticatedUser()` |
| `listMembersInOrganizationById()`         |
| `getMemberInOrganizationById()`           |
| `updateMemberInOrganizationById()`        |
| `removeMemberFromOrganizationById()`      |
| `setUserAsSsoMemberForOrganization()`     |
| `listSpacesForOrganizationMember()`       |
| `listTeamsInOrganizationById()`           |
| `createOrganizationTeam()`                |
| `getTeamInOrganizationById()`             |
| `updateTeamInOrganizationById()`          |
| `removeTeamFromOrganizationById()`        |
| `updateMembersInOrganizationTeam()`       |
| `listTeamMembersInOrganizationById()`     |
| `addMemberToOrganizationTeamById()`       |
| `deleteMemberFromOrganizationTeamById()`  |
| `inviteUsersToOrganization()`             |
| `joinOrganizationWithInvite()`            |
| `upgradeOrganizationPlan()`               |
| `getOrganizationBillingPortal()`          |
| `requestOrganizationUpgrade()`            |
| `transferOrganization()`                  |
| `searchOrganizationContent()`             |
| `listSpacesInOrganizationById()`          |
| `listCollectionsInOrganizationById()`     |
| `setupDirectorySync()`                    |
| `listDirectorySyncGroups()`               |
| `syncDirectorySyncGroupsToTeams()`        |

#### Urls <a href="#urls" id="urls"></a>

The following methods can be found on the `client.urls` object.
