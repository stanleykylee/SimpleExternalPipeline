#!groovy
properties([
    pipelineTriggers([
        triggers: [
            [
                $class: 'jenkins.triggers.ReverseBuildTrigger',
                upstreamProjects: "Folder/Upstream1",
                threshold: hudson.model.Result.SUCCESS
            ]
        ]
    ]),
    [$class: 'RebuildSettings', autoRebuild: false, rebuildDisabled: false]
])

node{
sh 'echo "success"'
}
