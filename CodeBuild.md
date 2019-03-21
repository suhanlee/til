# CodeBuild

### References
- https://docs.aws.amazon.com/cli/latest/reference/s3/index.html
- https://docs.aws.amazon.com/ko_kr/codebuild/latest/userguide/build-env-ref-env-vars.html
- https://gist.github.com/sardemff7/8770751
- https://gist.github.com/caspyin/2288960

```
# make PR on github
# trigger code build
- use CODEBUILD_SOURCE_VERSION env for make PR bucket and PR comment
# create s3 bucket and public hosting based on pr
$ aws s3api create-bucket --acl public-read --bucket [BUCKET_NAME] --region ap-northeast-2 --create-bucket-configuration LocationConstraint=ap-northeast-2

# comment on github pr thread

```
