# Updating the Status of a Specified Deployment<a name="cce_02_0130"></a>

## Function<a name="section49067544"></a>

This API is used to update the status of a specified Deployment in a specified namespace.

## URI<a name="section38954717"></a>

PATCH /apis/apps/v1/namespaces/\{namespace\}/deployments/\{name\}/status \(supports only 1.9\)

PATCH /apis/apps/v1beta1/namespaces/\{namespace\}/deployments/\{name\}/status \(supports only 1.7\)

PATCH /apis/extensions/v1beta1/namespaces/\{namespace\}/deployments/\{name\}/status \(Compatible\)

[Table 1](#d0e37132)  describes the parameters of this API.

**Table  1**  Parameter description

<a name="d0e37132"></a>
<table><thead align="left"><tr id="row55592481"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.2.4.1.1"><p id="p65652297517"><a name="p65652297517"></a><a name="p65652297517"></a>Parameters</p>
</th>
<th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.4.1.2"><p id="p165661629135114"><a name="p165661629135114"></a><a name="p165661629135114"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="62.629999999999995%" id="mcps1.2.4.1.3"><p id="p14567629115114"><a name="p14567629115114"></a><a name="p14567629115114"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row6885624"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p20864651"><a name="p20864651"></a><a name="p20864651"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.2 "><p id="p12315142"><a name="p12315142"></a><a name="p12315142"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p58002450"><a name="p58002450"></a><a name="p58002450"></a>Name of the Deployment.</p>
</td>
</tr>
<tr id="row52260006"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p5202061"><a name="p5202061"></a><a name="p5202061"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.2 "><p id="p18713817"><a name="p18713817"></a><a name="p18713817"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p39424242"><a name="p39424242"></a><a name="p39424242"></a>Object name and auth scope, such as for teams and projects.</p>
</td>
</tr>
<tr id="row19273863"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p17679037"><a name="p17679037"></a><a name="p17679037"></a>pretty</p>
</td>
<td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.2 "><p id="p22715892"><a name="p22715892"></a><a name="p22715892"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p28047955"><a name="p28047955"></a><a name="p28047955"></a>If 'true', then the output is pretty printed.</p>
</td>
</tr>
</tbody>
</table>

## Request<a name="section15048140"></a>

**Request parameters**:

For the description about the  **Content-Type**  message header, see section  [Patch Request Method Operation Description](patch-request-method-operation-description.md).

**Example request**:

```
Content-Type: application/merge-patch+json
[
    {
        "op": "add",
        "path": "/status/replicas",
        "value": 3
    }
]
```

## Response<a name="section1215532"></a>

**Response parameters:**

For the description about response parameters, see  [Table 2](creating-a-deployment.md#table12862324102610).

**Example response:**

```
{
    "kind": "Deployment",
    "apiVersion": "apps/v1beta1",
    "metadata": {
        "name": "deploy-12130306",
        "namespace": "ns-12130306-s",
        "selfLink": "/apis/apps/v1beta1/namespaces/ns-12130306-s/deployments/deploy-12130306/status",
        "uid": "27072a31-dfb3-11e7-9c19-fa163e2d897b",
        "resourceVersion": "418597",
        "generation": 2,
        "creationTimestamp": "2017-12-13T03:10:20Z",
        "labels": {
            "cce/appgroup": "deploy_test"
        },
        "annotations": {
            "deployment.kubernetes.io/revision": "1"
        },
        "enable": true
    },
    "spec": {
        "replicas": 1,
        "selector": {
            "matchLabels": {
                "cce/appgroup": "deploy_test"
            }
        },
        "template": {
            "metadata": {
                "creationTimestamp": null,
                "labels": {
            "cce/appgroup": "deploy_test"
                },
        "enable": true
    },
            "spec": {
                "containers": [
                    {
                        "name": "deploycon-12130306",
                        "image": "172.16.5.235:20202/test/redis:latest",
                        "resources": {},
                        "terminationMessagePath": "/dev/termination-log",
                        "terminationMessagePolicy": "File",
                        "imagePullPolicy": "IfNotPresent"
                    }
                ],
                "restartPolicy": "Always",
                "terminationGracePeriodSeconds": 30,
                "dnsPolicy": "ClusterFirst",
                "securityContext": {},
                "schedulerName": "default-scheduler"
            }
        },
        "strategy": {
            "type": "RollingUpdate",
            "rollingUpdate": {
                "maxUnavailable": "25%",
                "maxSurge": "25%"
            }
        },
        "revisionHistoryLimit": 2,
        "progressDeadlineSeconds": 600
    },
    "status": {
        "observedGeneration": 2,
        "replicas": 3,
        "updatedReplicas": 1,
        "readyReplicas": 1,
        "availableReplicas": 1,
        "conditions": [
            {
                "type": "Progressing",
                "status": "True",
                "lastUpdateTime": "2017-12-13T03:10:20Z",
                "lastTransitionTime": "2017-12-13T03:10:20Z",
                "reason": "NewReplicaSetAvailable",
                "message": "ReplicaSet \"deploy-12130306-3417241766\" has successfully progressed."
            },
            {
                "type": "Available",
                "status": "True",
                "lastUpdateTime": "2017-12-13T03:10:23Z",
                "lastTransitionTime": "2017-12-13T03:10:23Z",
                "reason": "MinimumReplicasAvailable",
                "message": "Deployment has minimum availability."
            }
        ]
    }
}
```

## Status Code<a name="section10939791"></a>

[Table 2](#d0e37225)  describes the status code of this API.

**Table  2**  Status code

<a name="d0e37225"></a>
<table><thead align="left"><tr id="row57629356"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p37466265"><a name="p37466265"></a><a name="p37466265"></a>Status Code</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p14868643"><a name="p14868643"></a><a name="p14868643"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row63509425"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p43989804"><a name="p43989804"></a><a name="p43989804"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p6404347"><a name="p6404347"></a><a name="p6404347"></a>This operation succeeds, and a Deployment resource object is returned.</p>
</td>
</tr>
</tbody>
</table>

For the description about status codes, see  [Status Code](status-code.md).

