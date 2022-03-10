# Includer

一个便捷的include的wrapper封装

## 安装

``` bash
composer require digphp/includer
```

## 用例

### 方式一

``` php
<?php
$phpcode='hello <?php echo $name;?>';
$name='xiaoming';
include \DigPHP\Includer\Wrapper::write($phpcode);
```

### 方式二

``` php
<?php
$phpcode='hello <?php echo $name;?>';
\DigPHP\Includer\Wrapper::load($phpcode, ['name'=>'xiaoming']);
```
