# KuaiDi100

PHP Wrapper for KuaiDi100.


## Installing

1. require library

```shell
composer require xu42/kuaidi100
```

## Usage

1. GeCode

```php
KuaiDi100::getCode('12303940284');
```

2. Track

```php
KuaiDi100::track('yunda', '12303940284');
```


3. exp

```php
namespace app\index\controller;

use Xu42\KuaiDi100\KuaiDi100;

/**
 * 测试任务
 */
class Excel
{

    public function index()
    {
        $logistics = KuaiDi100::getCode('634246542032');
        $data  = KuaiDi100::track($logistics, '634246542032');
        dump($data);
    }

}
```


## License

[MIT](LICENSE)
