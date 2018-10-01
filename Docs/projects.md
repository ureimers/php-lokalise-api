# Projects API

### List projects
https://lokalise.co/api2docs/php/#transition-list-all-projects-get

```php
$response = $client->projects->list(
    [
        'filter_team_id' => 1234,
        'limit' => 20,
        'page' => 1,
    ]
);
```

```php
$response = $client->projects->fetchAll(
    [
        'filter_team_id' => 1234,
    ]
);
```

### Create a project
https://lokalise.co/api2docs/php/#transition-create-a-project-post

```php
$response = $client->projects->create(
    [
        'name' => 'New project',
        'team_id' => 1234,
    ]
);
```

### Retrieve a project
https://lokalise.co/api2docs/php/#transition-retrieve-a-project-get

```php
$response = $client->projects->retrieve($projectId);
```

### Update a project
https://lokalise.co/api2docs/php/#transition-update-a-project-put

```php
$response = $client->projects->update(
    $projectId,
    [
        'name' => 'Old project',
    ]
);
```

### Empty a project
https://lokalise.co/api2docs/php/#transition-empty-a-project-put

```php
$response = $client->projects->empty($projectId);
```

### Delete a project
https://lokalise.co/api2docs/php/#transition-delete-a-project-delete

```php
$response = $client->projects->delete($projectId);
```