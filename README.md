<h1 style='margin: 30px 0px 0px; padding: 0px; color: rgb(23, 43, 77); font-size: 24px; line-height: 1; letter-spacing: -0.01em; font-weight: normal; text-transform: none; border-bottom-color: rgb(28, 57, 94); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; orphans: 2; text-align: start; text-indent: 0px; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;'><span style="font-size: 15px;"><strong>Introduction</strong></span></h1>
<p style='margin: 10px 0px 0px; padding: 0px; color: rgb(23, 43, 77); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial; line-height: 1;'><span style="font-size: 15px;">This Universal Task&nbsp;allows&nbsp;Stonebranch&nbsp;users&nbsp;to orchestrate, schedule, trigger, and monitor the Snowflake load and unload process from different data sources (cloud storage or local VM&rsquo;s) directly&nbsp;from Universal&nbsp;Controller. It uses Python libraries to perform all functions listed in the following sections. Alternatively, you also can perform all these operations using the snowflake JDBC driver which you can add to the Universal Controller libraries, and use SQL Task to perform any operations with Snowflake (<a class="external-link" href="https://docs.snowflake.com/en/user-guide/jdbc-download.html" rel="nofollow" style="color: rgb(0, 82, 204); text-decoration: none;">https://docs.snowflake.com/en/user-guide/jdbc-download.html</a>)</span></p>
<h1 style='margin: 30px 0px 0px; padding: 0px; color: rgb(23, 43, 77); font-size: 24px; line-height: 1; letter-spacing: -0.01em; font-weight: normal; text-transform: none; border-bottom-color: rgb(28, 57, 94); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; orphans: 2; text-align: start; text-indent: 0px; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;'><span style="font-size: 15px;"><strong>Overview</strong></span></h1>
<p style='margin: 10px 0px 0px; padding: 0px; color: rgb(23, 43, 77); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial; line-height: 1;'><span style="font-size: 15px;">Users can orchestrate the Snowflake functionalities using the following features available in the Universal Task</span></p>
<ul class="ak-ul" style='margin: 10px 0px 0px; list-style-type: disc; color: rgb(23, 43, 77); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;'>
    <li>
        <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">UAC functionalities (Snowflake -Loading)</span></p>
        <ul class="ak-ul" style="margin: 0px; list-style-type: disc;">
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Load data from AWS S3 to Snowflake.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Load data from Azure Storage to Snowflake.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Load data from Google storage to Snowflake.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Load Internal stage file to Snowflake Table.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Copy from local server to Internal staging.</span></p>
            </li>
        </ul>
    </li>
    <li>
        <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">UAC functionalities (Snowflake - Unloading)</span></p>
        <ul class="ak-ul" style="margin: 0px; list-style-type: disc;">
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Unload Snowflake data to AWS S3.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Unload Snowflake data to Azure Storage.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Unload Snowflake data to Google Storage.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Unload &nbsp;Snowflake data to Internal stage.</span></p>
            </li>
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Unload from internal stage to local server.</span></p>
            </li>
        </ul>
    </li>
    <li>
        <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">UAC functionalities (Snowflake &ndash; Execute Commands)</span></p>
        <ul style="margin: 0px; list-style-type: disc;">
            <li>
                <p style="margin: 0px; padding: 0px; line-height: 1;"><span style="font-size: 15px;">Execute a Snowflake command.</span></p>
            </li>
        </ul>
    </li>
</ul>
<h1 style='margin: 30px 0px 0px; padding: 0px; color: rgb(23, 43, 77); font-size: 24px; line-height: 1; letter-spacing: -0.01em; font-weight: normal; text-transform: none; border-bottom-color: rgb(28, 57, 94); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; orphans: 2; text-align: start; text-indent: 0px; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;'><span style="font-size: 15px;"><strong>Software Requirements</strong></span></h1>
<p style='margin: 10px 0px 0px; padding: 0px; color: rgb(23, 43, 77); font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial; line-height: 1;'><span style="font-size: 15px;">This integration requires a Universal Agent and a Python runtime to execute the Universal Task against Snowflake.</span></p>

<p>&nbsp;</p>
Please visit this link to find key features, prerequisites, installation instructions, configuration instructions, and examples of how to use this integration. 
<a href="https://docs.stonebranch.com/confluence/display/UC69/UAC+-+Snowflake">UAC - Snowflake</a>.&nbsp;</li>

