## Component Information

| Field Name               | Value                            |
|:--------------------------|:---------------------------------|
| **Name**                 | ${{ values.name }}               |
| **Description**          | ${{ values.description }}        |
| **Domain**               | ${{ values.domain }}             |
| **Data Product**         | ${{ values.dataproduct }}        |
| **Identifier**           | ${{ values.identifier }}         |
| **Component Owner**      | ${{ values.owner }}              |
| **Depends On**           | ${{ values.dependsOn }}          |

## Vast deployment information

| Field Name        | Value                     |
|:--------------------|:---------------------------|
| **Database Name** | ${{ values.database_name }} |
| **Schema Name**   | ${{ values.schema_name }}   |
| **Table Name**    | ${{ values.table_name }}    |
| **S3 Path**       | ${{ values.path }}          |
| **Policy Name**   | ${{ values.policy_name }}   |
| **Bucket Name**   | ${{ values.bucket_name }}   |
| **Vip Pool**      | ${{ values.vip_pool }}      |

## Schema

| Column Name | Data Type | Length | Data Type Display | Array Element Type | Description |
|:-------------|:-----------|:-------|:------------------|:------------------|:--------------|
{% if values.schemaColumns | length > 0 %}{% for column in values.schemaColumns %}| ${{ column.name }} | ${{ column.dataType }} | ${{ column.dataLength }} | ${{ column.dataTypeDisplay }} | ${{ column.arrayDataType }} | ${{ column.description }} |
{% endfor %}{% else %}| _No columns defined_ | | | | |
{% endif %}