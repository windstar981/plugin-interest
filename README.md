**Cách chạy** <br>

``cd platform``

``git submodule add https://github.com/windstar981/plugin-interest``

Thêm vào repositories của project chính(thay đổi index 0 cho phù hợp)
``
    "repositories": {
            "0": {
                "type": "path",
                "url": "./platform/plugin-interest",
                "options": {
                    "symlink": true
                }
            }
        }
``

``composer require tool/plugininterest``

Cop mục css, js ra public theo đường dẫn

``public\platform\plugin``

Include css ở file header

``@include('plugin-interest::includecss')``

Include js ở file footer

``@include('plugin-interest::includejs')``
