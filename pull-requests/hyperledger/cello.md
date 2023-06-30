---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    Listed the commands that are not working
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1: make start: This command starts the service, but it doesn't specify which service to start. It relies on the start-docker-compose rule, which starts the services defined in the bootup/docker-compose-files/${COMPOSE_FILE} file. However, the value of ${COMPOSE_FILE} is determined by the MODE variable, which is set to prod by default. If you want to use this command, ensure that the appropriate value is set for ${COMPOSE_FILE} and that the necessary configuration files are present.

2: make stop: This command stops the service, but it doesn't specify which service to stop. It relies on the stop-docker-compose rule, which stops the services defined in the bootup/docker-compose-files/${COMPOSE_FILE} file. Similar to the start command, ensure that the value of ${COMPOSE_FILE} is correctly set.

3: make restart: This command restarts the services, but it relies on the stop and start commands. As mentioned above, ensure that the necessary configurations are in place for those commands to work correctly.

4: make clean-images: This command is intended to clean all Cello-related Docker images. However, it executes the clean rule, which stops services and cleans Docker containers. It doesn't specifically target cleaning Docker images. If you want to clean Docker images, you may need to modify the command to remove the images instead of stopping services and cleaning containers.

5: make check-dashboard: This command checks the dashboard but relies on the docker-compose command with a specific configuration file. Ensure that the necessary configuration files are present and correctly set up for the dashboard check to work as expected.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 11:12:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/530" class=".btn">#530</a>
            </td>
            <td>
                <b>
                    Fix make command error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed the nested dependency version issue, mentioned in #528.

Fixed the code style issues found by Flake8.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 06:34:05 +0000 UTC
    </div>
</div>

