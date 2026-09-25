## Component Information

| Field Name               | Value                            |
|:--------------------------|:---------------------------------|
| **Name**                 | ${{ values.name }}               |
| **Fully Qualified Name** | ${{ values.fullyQualifiedName }} |
| **Description**          | ${{ values.description }}        |
| **Domain**               | ${{ values.domain }}             |
| **Data Product**         | ${{ values.dataproduct }}        |
| **Identifier**           | ${{ values.identifier }}         |
| **Component Owner**      | ${{ values.owner }}              |
| **Depends On**           | ${{ values.dependsOn }}          |

## Terms and Conditions & SLA

| Field name               | Value                             |
|:--------------------------|:----------------------------------|
| **Terms and Conditions** | ${{ values.termsAndConditions }} |
| **Interval of change**   | ${{ values.intervalOfChange }}   |
| **Timeliness**           | ${{ values.timeliness }}         |
| **Uptime**               | ${{ values.upTime }}             |

## Data Sharing Agreement

| Field name          | Value                          |
|:---------------------|:--------------------------------|
| **Purpose**         | ${{ values.purpose }}         |
| **Billing**         | ${{ values.billing }}         |
| **Security**        | ${{ values.security }}        |
| **Intended Usage**  | ${{ values.intendedUsage }}   |
| **Limitations**     | ${{ values.limitations }}     |
| **Lifecycle**       | ${{ values.lifeCycle }}       |
| **Confidentiality** | ${{ values.confidentiality }} |

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

| Column Name | Data Type | Description |
|:-------------|:-----------|:--------------|
{% if values.schemaColumns | length > 0 %}{% for column in values.schemaColumns %}| ${{ column.name }} | ${{ column.dataType }} | ${{ column.description }} |
{% endfor %}{% else %}| _No columns defined_ | | |
{% endif %}

