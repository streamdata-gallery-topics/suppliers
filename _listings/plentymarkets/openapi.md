swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/{id}/variations/{variationId}/variation_suppliers:
    post:
      summary: Create a link between variation and supplier
      description: Creates a link between a variation and a supplier and adds supplier
        data.
      operationId: postRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Supplier
    get:
      summary: Lists suppliers for a variation
      description: Lists all supplier data linked to a variation. The ID of the variation
        must be specified.
      operationId: getRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suppliersa
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_suppliers/{variationSupplierId}:
    delete:
      summary: Delete link between variation and supplier
      description: Deletes a link between a variation and a supplier. The ID of the
        variation and the ID of the link between the variation and the supplier must
        be specified.
      operationId: deleteRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Supplier
    get:
      summary: Get supplier data for a variation
      description: Gets the data for a supplier linked to a variation. The ID of the
        variation and the ID of the link between the variation and the supplier must
        be specified.
      operationId: getRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - Supplier
      - Dataa
      - Variation
    put:
      summary: Updates supplier data for a variation
      description: Updates the data of a supplier linked to a variation.
      operationId: putRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - S
      - Supplier
      - Dataa
      - Variation