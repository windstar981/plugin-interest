**Cách chạy** <br>

``cd platform``

``git submodule add https://github.com/windstar981/plugin-interest``

Thêm vào repositories của project chính(thay đổi index 0 cho phù hợp)<br>
``
    "repositories": { <br>
            "0": { <br>
                "type": "path", <br>
                "url": "./platform/plugin-interest", <br>
                "options": { <br>
                    "symlink": true <br>
                } <br>
            } <br>
        } <br>
``

``composer require tool/plugininterest``

Cop mục css, js ra public theo đường dẫn

``public\platform\plugin``

Include css ở file header

``@include('plugin-interest::includecss')``

Include js ở file footer

``@include('plugin-interest::includejs')``
