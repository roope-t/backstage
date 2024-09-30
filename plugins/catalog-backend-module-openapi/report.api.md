## API Report File for "@backstage/plugin-catalog-backend-module-openapi"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { BackendFeature } from '@backstage/backend-plugin-api';
import { CatalogProcessor } from '@backstage/plugin-catalog-node';
import { Config } from '@backstage/config';
import { Entity } from '@backstage/catalog-model';
import { JsonValue } from '@backstage/types';
import { LocationSpec } from '@backstage/plugin-catalog-common';
import { Logger } from 'winston';
import { PlaceholderResolverParams } from '@backstage/plugin-catalog-backend';
import { ScmIntegrations } from '@backstage/integration';
import { UrlReaderService } from '@backstage/backend-plugin-api';

// @public
const catalogModuleJsonSchemaRefPlaceholderResolver: BackendFeature;
export default catalogModuleJsonSchemaRefPlaceholderResolver;

// @public (undocumented)
export function jsonSchemaRefPlaceholderResolver(
  params: PlaceholderResolverParams,
): Promise<JsonValue>;

// @public @deprecated (undocumented)
export const openApiPlaceholderResolver: typeof jsonSchemaRefPlaceholderResolver;

// @public @deprecated (undocumented)
export class OpenApiRefProcessor implements CatalogProcessor {
  constructor(options: {
    integrations: ScmIntegrations;
    logger: Logger;
    reader: UrlReaderService;
  });
  // (undocumented)
  static fromConfig(
    config: Config,
    options: {
      logger: Logger;
      reader: UrlReaderService;
    },
  ): OpenApiRefProcessor;
  // (undocumented)
  getProcessorName(): string;
  // (undocumented)
  preProcessEntity(entity: Entity, location: LocationSpec): Promise<Entity>;
}

// Warnings were encountered during analysis:
//
// src/OpenApiRefProcessor.d.ts:12:1 - (ae-undocumented) Missing documentation for "OpenApiRefProcessor".
// src/OpenApiRefProcessor.d.ts:16:5 - (ae-undocumented) Missing documentation for "fromConfig".
// src/OpenApiRefProcessor.d.ts:25:5 - (ae-undocumented) Missing documentation for "getProcessorName".
// src/OpenApiRefProcessor.d.ts:26:5 - (ae-undocumented) Missing documentation for "preProcessEntity".
// src/index.d.ts:8:22 - (ae-undocumented) Missing documentation for "openApiPlaceholderResolver".
// src/jsonSchemaRefPlaceholderResolver.d.ts:4:1 - (ae-undocumented) Missing documentation for "jsonSchemaRefPlaceholderResolver".

// (No @packageDocumentation comment for this package)
```