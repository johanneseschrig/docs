<!-- this file is automatically generated and updated by a github action -->
<pre class="log">
> cds add --help

<strong>SYNOPSIS</strong>
    <em>cds add</em> &lt;feature | comma-separated list of features&gt;

    Add one or more features to an existing project - grow as you go.

    Pick any of these:

      <em>completion</em>                   - shell completion for cds commands
      <em>tiny-sample</em>                  - add minimal sample files
      <em>sample</em>                       - add sample files including Fiori UI
      <em>mta</em>                          - Cloud Foundry deployment using mta.yaml
      <em>cf-manifest</em>                  - Cloud Foundry deployment using manifest files
      <em>helm</em>                         - Kyma deployment using Helm charts
      <em>helm-unified-runtime</em>         - Kyma deployment using Unified Runtime Helm charts
      <em>containerize</em>                 - containerization using ctz CLI
      <em>multitenancy</em>                 - schema-based multitenancy support
      <em>toggles</em>                      - allow dynamically toggled features
      <em>extensibility</em>                - tenant-specific model extensibility
      <em>side-by-side-extensibility</em>   - logic extensibility via extension points
      <em>mtx</em>                          - multitenancy + toggles + extensibility
      <em>xsuaa</em>                        - authentication via XSUAA
      <em>hana</em>                         - database support for SAP HANA
      <em>postgres</em>                     - database support for PostgreSQL
      <em>sqlite</em>                       - database support for SQLite
      <em>h2</em>                           - database support for H2
      <em>liquibase</em>                    - database migration using Liquibase
      <em>redis</em>                        - SAP BTP Redis, Hyperscaler Option
      <em>attachments</em>                  - SAP BTP Object Store Service
      <em>malware-scanner</em>              - SAP Malware Scanning Service
      <em>local-messaging</em>              - messaging via local event bus
      <em>file-based-messaging</em>         - messaging via file system
      <em>enterprise-messaging</em>         - messaging via SAP Enterprise Messaging
      <em>enterprise-messaging-shared</em>  - messaging via shared SAP Enterprise Messaging
      <em>redis-messaging</em>              - messaging via Redis
      <em>kafka</em>                        - messaging via Apache Kafka
      <em>approuter</em>                    - dynamic routing using @sap/approuter
      <em>connectivity</em>                 - SAP BTP Connectivity Service
      <em>destination</em>                  - SAP BTP Destination Service
      <em>html5-repo</em>                   - SAP BTP HTML5 Application Repository
      <em>portal</em>                       - SAP BTP Portal Service
      <em>application-logging</em>          - SAP BTP Application Logging Service
      <em>audit-logging</em>                - SAP BTP Audit Logging Service
      <em>notifications</em>                - SAP BTP Notification Service
      <em>workzone-standard</em>            - SAP BTP Work Zone, Standard Edition
      <em>data</em>                         - add CSV headers for modeled entities
      <em>http</em>                         - add .http files for modeled services
      <em>lint</em>                         - configure cds lint
      <em>pipeline</em>                     - CI/CD pipeline integration
      <em>typer</em>                        - type generation for CDS models
      <em>typescript</em>                   - add minimum configuration for a bare TypeScript project
      <em>handler</em>                      - handler stubs for service entities, actions and functions

<strong>OPTIONS</strong>
    <em>--for | -4</em> &lt;profile&gt;

      Write configuration data for the given profile.

    <em>--force</em>

      Overwrite all files in case the target files already exist.

    <em>--package</em> &lt;name&gt;

      Pull a package from your npm registry.


<strong>FEATURE OPTIONS</strong>
    <em>cds add audit-logging</em>

      --plan

        Specify the service plan.

    <em>cds add cloud-logging</em>

      --plan

        Override the service plan used for the MTA generation.

      --with-telemetry

        Add telemetry capabilities.

    <em>cds add completion</em>

      --shell | -s

        &lt;optional&gt; Forces completion setup for a given shell and disables auto detection.
        Usually the shell is determined automatically and this is only for cases where the automatic
        detection fails. Valid values: bash, fish, gitbash, ps, zsh.

    <em>cds add data</em>

      --filter | -f

        Filter for entities matching the given pattern. If it contains meta
        characters like '^' or '*', it is treated as a regular expression,
        otherwise as an include pattern, i.e /.*pattern.*/i

      --data:for

        Deprecated. Use '--filter' instead.

      --records | -n

        The number of records to be created for each entity.

      --content-type | -c

        The content type of the data. One of "json" or "csv".

      --out | -o

        The output target folder.

    <em>cds add enterprise-messaging</em>

      --cloudevents | -c

        Use CloudEvents formatting.

    <em>cds add enterprise-messaging-shared</em>

      --cloudevents | -c

        Use CloudEvents formatting.

    <em>cds add handler</em>

      --filter | -f

        Filter for entities, actions or functions matching the given pattern.
        For Node.js, if it contains meta characters like '^' or '*', it is treated as a regular expression,
        otherwise as an include pattern, i.e /.*bookshop.*/i
        For Java, only '*' and '**' as suffix wildcards are allowed, as in 'my.bookshop.*' or 'my.**'

      --out | -o

        Custom output directory.
        For Java, the default is 'handlers'. For Node.js, the default is 'srv'.

    <em>cds add helm</em>

      --y

        If provided, the default values will be used for all prompts.

    <em>cds add http</em>

      --filter | -f

        Filter for services or entities or actions matching the given pattern. If it contains meta
        characters like '^' or '*', it is treated as a regular expression,
        otherwise as an include pattern, i.e /.*pattern.*/i

      --for-app | -a

        Specify the name of the app to generate requests for.
        If not specified, localhost and default auth will be used.

      --out | -o

        The output directory.
        By default, an `http` dir is created in either `test/`, `tests/`, `__tests__/`, or at the root level.

      --dry

        Print the generated requests to the console instead of writing them to a file.


<strong>EXAMPLES</strong>
    <em>cds add</em> sample
    <em>cds add</em> multitenancy,hana,xsuaa --for production
    <em>cds add</em> data --filter my.namespace.MyEntity
    <em>cds add</em> mta
    <em>cds add</em> helm


<strong>SEE ALSO</strong>
  <em>cds init</em>
</pre>