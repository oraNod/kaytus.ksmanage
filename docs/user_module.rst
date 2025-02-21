.. Document meta

:orphan:

.. Anchors

.. _ansible_collections.kaytus.ksmanage.user_module:

.. Anchors: short name for ansible.builtin

.. Anchors: aliases



.. Title

kaytus.ksmanage.user -- Manage user
+++++++++++++++++++++++++++++++++++

.. Collection note

.. note::
    This plugin is part of the `kaytus.ksmanage collection <https://galaxy.ansible.com/kaytus/ksmanage>`_.

    To install it use: :code:`ansible-galaxy collection install kaytus.ksmanage`.

    To use it in a playbook, specify: :code:`kaytus.ksmanage.user`.

.. version_added

.. versionadded:: 1.0.0 of kaytus.ksmanage

.. contents::
   :local:
   :depth: 1

.. Deprecated


Synopsis
--------

.. Description

- Manage user on kaytus Server.


.. Aliases


.. Requirements

Requirements
------------
The below requirements are needed on the host that executes this module.

- Python 3.7+
- inManage


.. Options

Parameters
----------

.. raw:: html

    <table  border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="2">Parameter</th>
            <th>Choices/<font color="blue">Defaults</font></th>
                        <th width="100%">Comments</th>
        </tr>
                    <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-access"></div>
                    <b>access</b>
                    <a class="ansibleOptionLink" href="#parameter-access" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li>enable</li>
                                                                                                                                                                                                <li>disable</li>
                                                                                    </ul>
                                                                            </td>
                                                                <td>
                                            <div>User access.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-email"></div>
                    <b>email</b>
                    <a class="ansibleOptionLink" href="#parameter-email" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>User email.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-host"></div>
                    <b>host</b>
                    <a class="ansibleOptionLink" href="#parameter-host" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Specifies the DNS host name or address for connecting to the remote device over the specified transport.  The value of host is used as the destination address for the transport.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-password"></div>
                    <b>password</b>
                    <a class="ansibleOptionLink" href="#parameter-password" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Specifies the password to use to authenticate the connection to the remote device. If the value is not specified in the task, the value of environment variable <code>ANSIBLE_NET_PASSWORD</code> will be used instead.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-priv"></div>
                    <b>priv</b>
                    <a class="ansibleOptionLink" href="#parameter-priv" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=string</span>                                            </div>
                                                        </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li>kvm</li>
                                                                                                                                                                                                <li>vmm</li>
                                                                                                                                                                                                <li>sol</li>
                                                                                                                                                                                                <li>none</li>
                                                                                    </ul>
                                                                            </td>
                                                                <td>
                                            <div>Other user permissions, select one or more from None/KVM/VMM/SOL.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-provider"></div>
                    <b>provider</b>
                    <a class="ansibleOptionLink" href="#parameter-provider" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">dictionary</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>A dict object containing connection details.</div>
                                                        </td>
            </tr>
                                        <tr>
                                                    <td class="elbow-placeholder"></td>
                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-provider/host"></div>
                    <b>host</b>
                    <a class="ansibleOptionLink" href="#parameter-provider/host" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Specifies the DNS host name or address for connecting to the remote device over the specified transport.  The value of host is used as the destination address for the transport.</div>
                                                        </td>
            </tr>
                                <tr>
                                                    <td class="elbow-placeholder"></td>
                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-provider/password"></div>
                    <b>password</b>
                    <a class="ansibleOptionLink" href="#parameter-provider/password" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Specifies the password to use to authenticate the connection to the remote device. If the value is not specified in the task, the value of environment variable <code>ANSIBLE_NET_PASSWORD</code> will be used instead.</div>
                                                        </td>
            </tr>
                                <tr>
                                                    <td class="elbow-placeholder"></td>
                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-provider/username"></div>
                    <b>username</b>
                    <a class="ansibleOptionLink" href="#parameter-provider/username" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Configures the username to use to authenticate the connection to the remote device. If the value is not specified in the task, the value of environment variable <code>ANSIBLE_NET_USERNAME</code> will be used instead.</div>
                                                        </td>
            </tr>
                    
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-role_id"></div>
                    <b>role_id</b>
                    <a class="ansibleOptionLink" href="#parameter-role_id" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>User group.</div>
                                            <div>Default user group &#x27;Administrator&#x27;, &#x27;Operator&#x27;, &#x27;User&#x27;.</div>
                                            <div>Use command <code>user_group_info</code> can get all group information.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-state"></div>
                    <b>state</b>
                    <a class="ansibleOptionLink" href="#parameter-state" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li><div style="color: blue"><b>present</b>&nbsp;&larr;</div></li>
                                                                                                                                                                                                <li>absent</li>
                                                                                    </ul>
                                                                            </td>
                                                                <td>
                                            <div>Whether the user should exist or not, taking action if the state is different from what is stated.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-uid"></div>
                    <b>uid</b>
                    <a class="ansibleOptionLink" href="#parameter-uid" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">integer</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>User id,The range is 1 to 16.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-uname"></div>
                    <b>uname</b>
                    <a class="ansibleOptionLink" href="#parameter-uname" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>User name,Required when uid is None.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-upass"></div>
                    <b>upass</b>
                    <a class="ansibleOptionLink" href="#parameter-upass" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>User password.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-username"></div>
                    <b>username</b>
                    <a class="ansibleOptionLink" href="#parameter-username" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Configures the username to use to authenticate the connection to the remote device. If the value is not specified in the task, the value of environment variable <code>ANSIBLE_NET_USERNAME</code> will be used instead.</div>
                                                        </td>
            </tr>
                        </table>
    <br/>

.. Notes

Notes
-----

.. note::
   - Does not support ``check_mode``.

.. Seealso


.. Examples

Examples
--------

.. code-block:: yaml+jinja

    
    - name: User test
      hosts: ksmanage
      no_log: true
      connection: local
      gather_facts: no
      vars:
        ksmanage:
          host: "{{ ansible_ssh_host }}"
          username: "{{ username }}"
          password: "{{ password }}"

      tasks:

      - name: "Add user"
        kaytus.ksmanage.user:
          state: "present"
          uname: "wbs"
          upass: "admin"
          role_id: "Administrator"
          priv: "kvm,sol"
          email: "wbs@ieisystem.com"
          provider: "{{ ksmanage }}"

      - name: "Set user"
        kaytus.ksmanage.user:
          state: "present"
          uname: "wbs"
          upass: "12345678"
          role_id: "user"
          priv: "kvm,sol"
          provider: "{{ ksmanage }}"




.. Facts


.. Return values

Return Values
-------------
Common return values are documented :ref:`here <common_return_values>`, the following are the fields unique to this module:

.. raw:: html

    <table border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="1">Key</th>
            <th>Returned</th>
            <th width="100%">Description</th>
        </tr>
                    <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-changed"></div>
                    <b>changed</b>
                    <a class="ansibleOptionLink" href="#return-changed" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">boolean</span>
                                          </div>
                                    </td>
                <td>always</td>
                <td>
                                            <div>Check to see if a change was made on the device.</div>
                                        <br/>
                                    </td>
            </tr>
                                <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-message"></div>
                    <b>message</b>
                    <a class="ansibleOptionLink" href="#return-message" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">string</span>
                                          </div>
                                    </td>
                <td>always</td>
                <td>
                                            <div>Messages returned after module execution.</div>
                                        <br/>
                                    </td>
            </tr>
                                <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-state"></div>
                    <b>state</b>
                    <a class="ansibleOptionLink" href="#return-state" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">string</span>
                                          </div>
                                    </td>
                <td>always</td>
                <td>
                                            <div>Status after module execution.</div>
                                        <br/>
                                    </td>
            </tr>
                        </table>
    <br/><br/>

..  Status (Presently only deprecated)


.. Authors

Authors
~~~~~~~

- WangBaoshan (@ieisystem)



.. Parsing errors

