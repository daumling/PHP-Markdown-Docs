# PHP Class Markdown Documentation

Version: 0.1.11 beta

Github: https://github.com/marcocesarato/PHP-Class-Markdown-Docs

Author: Marco Cesarato

## Description

This package can convert PHPDoc comments from classes into Markdown.

It can parse a class file with a given file name and extracts the documentation of its functions and variables that it may contain in PHPDoc format.

The package can convert the extracted documentation into a file in Markdown format.

## Install

### Composer
1. Install composer
2. Type `composer require marcocesarato/markdown`
4. Enjoy

## Methods

| Method        | Description                        | Type                | Parameters | Return |
| ------------- | ---------------------------------- | ------------------- | ---------- | ------ |
| getMarkdown   | Get markdown class documentation   | public<br>static    | $file      | string |
| printMarkdown | Print Markdown class documentation | public<br>static    | $file      |        |
| getArray      | Get php array class documentation  | public<br>static    | $file      | array  |

## Example

### Usage

```php
Markdown::printMarkdown('Sample.php');
```


#### Output Text

```text
## CoreClass
| Method        | Description                                        | Type   | Parameters                                         | Return         |
| ------------- | -------------------------------------------------- | ------ | -------------------------------------------------- | -------------- |
| __construct   | Constructor                                        | public |                                                    |                |
| __init        | Initialize                                         |        |                                                    | bool           |
| CoreClass     | Constructor                                        |        |                                                    |                |
| getInstance   | Get singleton instance                             |        |                                                    | CoreClass      |
| apply_filters | Apply module hook filters                          |        | $name<br>$data                                     | mixed          |
| do_action     | Do module hook actions                             |        | $name                                              | bool           |
| add_action    | Add module hook action                             |        | $name<br>$action                                   | bool           |
| add_filter    | Add module hook filter                             |        | $name<br>$filter                                   | bool           |
| add_request   | Add Ajax request                                   |        | $name<br>$request<br>bool $public                  | bool           |
| exists        | Check if element already exists if exists it will be updated on Save else it will be inserted |        | null $what<br>bool $undelete                       | bool           |
| prepare       | Prepare retrieve conditions                        |        | null $what<br>null $operators                      | array          |
| retrieve      | Retrieve element                                   |        | null $what<br>bool $encode<br>null $onlyFields<br>null $orderBy<br>bool $returnAsArray<br>null $operators<br>bool $dump | array<br>mixed |
| fetch         |                                                    |        | $what<br>null $operators                           | array          |
```

#### Markdown Result

## CoreClass
| Method        | Description                                        | Type   | Parameters                                         | Return         |
| ------------- | -------------------------------------------------- | ------ | -------------------------------------------------- | -------------- |
| __construct   | Constructor                                        | public |                                                    |                |
| __init        | Initialize                                         |        |                                                    | bool           |
| CoreClass     | Constructor                                        |        |                                                    |                |
| getInstance   | Get singleton instance                             |        |                                                    | CoreClass      |
| apply_filters | Apply module hook filters                          |        | $name<br>$data                                     | mixed          |
| do_action     | Do module hook actions                             |        | $name                                              | bool           |
| add_action    | Add module hook action                             |        | $name<br>$action                                   | bool           |
| add_filter    | Add module hook filter                             |        | $name<br>$filter                                   | bool           |
| add_request   | Add Ajax request                                   |        | $name<br>$request<br>bool $public                  | bool           |
| exists        | Check if element already exists if exists it will be updated on Save else it will be inserted |        | null $what<br>bool $undelete                       | bool           |
| prepare       | Prepare retrieve conditions                        |        | null $what<br>null $operators                      | array          |
| retrieve      | Retrieve element                                   |        | null $what<br>bool $encode<br>null $onlyFields<br>null $orderBy<br>bool $returnAsArray<br>null $operators<br>bool $dump | array<br>mixed |
| fetch         |                                                    |        | $what<br>null $operators                           | array          |
