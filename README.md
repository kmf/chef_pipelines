# Chef Pipelines

## InSpec Pipeline

### Description

### Depends On (Up stream)
- Other InSpec Pipelines (Optional)

### Depends On It (Down stream)
- Policyfile Pipeline (Mandatory)

![InSpec Pipeline](/images/inspec_pipeline.png)

### Code
https://github.com/anthonygrees/inspec_pipeline

## Cookbook Pipeline

### Description

### Depends On (Up stream)
- Other Cookbook Pipelines (Optional)

### Depends On It (Down stream)
- Policyfile Pipeline (Mandatory)

![Cookbook Pipeline](/images/cookbook_pipeline.png)

### Code
https://github.com/anthonygrees/cookbook_pipeline

## Policyfile Pipeline

### Description

### Depends On (Up stream)
- InSpec Pipeline (Mandatory)
- Cookbook Pipeline (Mandatory)

### Depends On It (Down stream)
- Image Pipeline (Mandatory)
- Existing Brownfields Recovery Pipeline (Mandatory)

![Cookbook Pipeline](/images/policyfile_pipeline.png)

### Code
https://github.com/anthonygrees/policyfile_pipeline

## Image Pipeline

### Description

### Depends On (Up stream)
- Policyfile Pipeline (Mandatory)

### Depends On It (Down stream)
- All Provisioning Pipelines (Mandatory)

![Cookbook Pipeline](/images/image_pipeline.png)

### Code
https://github.com/anthonygrees/image_pipeline


## License and Author

* Author:: Matt Ray <matt@chef.io>
*       :: Anthony Rees <anthony@chef.io>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
