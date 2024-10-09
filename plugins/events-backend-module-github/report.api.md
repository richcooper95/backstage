## API Report File for "@backstage/plugin-events-backend-module-github"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { Config } from '@backstage/config';
import { EventParams } from '@backstage/plugin-events-node';
import { EventsService } from '@backstage/plugin-events-node';
import { RequestValidator } from '@backstage/plugin-events-node';
import { SubTopicEventRouter } from '@backstage/plugin-events-node';

// @public
export function createGithubSignatureValidator(
  config: Config,
): RequestValidator;

// @public
export class GithubEventRouter extends SubTopicEventRouter {
  constructor(options: { events: EventsService });
  // (undocumented)
  protected determineSubTopic(params: EventParams): string | undefined;
  // (undocumented)
  protected getSubscriberId(): string;
}

// Warnings were encountered during analysis:
//
// src/router/GithubEventRouter.d.ts:13:5 - (ae-undocumented) Missing documentation for "getSubscriberId".
// src/router/GithubEventRouter.d.ts:14:5 - (ae-undocumented) Missing documentation for "determineSubTopic".
```