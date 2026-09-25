<p align="center">
    <a href="https://www.witboost.com/">
        <img src="docs/img/witboost_logo.svg" alt="witboost" width=600 >
    </a>
</p>

Designed by [Agile Lab](https://www.agilelab.it/), Witboost is a versatile platform that addresses a wide range of sophisticated data engineering challenges. It enables businesses to discover, enhance, and productize their data, fostering the creation of automated data platforms that adhere to the highest standards of data governance. Want to know more about Witboost? Check it out [here](https://witboost.com/platform) or [contact us!](https://witboost.com/contact-us)

# Vast SQL Output Port Template

- [Overview](#overview)
- [Usage](#usage)

## Overview

Use this template to create an Output Port backed by a table on the [VAST Data](https://www.vastdata.com/) platform. The Output Port is implemented as a SQL table, created with the exact columns defined in the Data Contract schema declared during creation.

> Before using this template, replace the placeholder GitLab group (`your-gitlab-group`) in [`template.yaml`](./template.yaml) with the GitLab group that should own the repositories created by this template.

### What's a Template?

A Template is a tool that helps create components inside a Data Mesh. Templates help establish a standard across the organization. This standard leads to easier understanding, management and maintenance of components. Templates provide a predefined structure so that developers don't have to start from scratch each time, which leads to faster development and allows them to focus on other aspects, such as testing and business logic.

For more information, please refer to the [official documentation](https://docs.witboost.com/docs/data-teams/p6_advanced/p6_1_templates#getting-started).

This template uses Skeleton Entities.

### What's an Output Port?

An Output Port refers to the interface that a Data Product uses to provide data to other components or systems within the organization. The methods of data sharing can range from APIs to file exports and database links.

### VAST Data

VAST Data is a unified storage and data platform designed to remove the traditional trade-offs between performance, capacity and cost for large-scale, all-flash environments. Its Database engine exposes a transactional, schema-based SQL layer directly on top of the platform's data store, allowing structured tables to be created, queried and updated without a separate data warehouse.

Learn more about it on the [official website](https://www.vastdata.com/).

## Usage

To get information on how to use this template, refer to this [document](./docs/index.md).

## License

This project is available under the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-2.0); see [LICENSE](LICENSE) for full details.

## About Witboost

[Witboost](https://witboost.com/) is a cutting-edge Data Experience platform, that streamlines complex data projects across various platforms, enabling seamless data production and consumption. This unified approach empowers you to fully utilize your data without platform-specific hurdles, fostering smoother collaboration across teams.

It seamlessly blends business-relevant information, data governance processes, and IT delivery, ensuring technically sound data projects aligned with strategic objectives. Witboost facilitates data-driven decision-making while maintaining data security, ethics, and regulatory compliance.

Moreover, Witboost maximizes data potential through automation, freeing resources for strategic initiatives. Apply your data for growth, innovation and competitive advantage.

[Contact us](https://witboost.com/contact-us) or follow us on:

- [LinkedIn](https://www.linkedin.com/showcase/witboost/)
- [YouTube](https://www.youtube.com/@witboost-platform)

