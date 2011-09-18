# Title

*Simple HTML `<title>` generator*


****

## Installation
1. Copy *libraries & config* folder to your *application* folder
2. Edit *title.php* in config folder

## How to use
In your routes.php (or custom routes file), add a title using Title::put()

    'GET /home/dashboard/edit_profile' => function()
    {
        Title::put('My Dashboard');
        return View::make('dashboard/edit_profile');
    }


Next, in your view file, call `<?=Title::get()?>` to generate title.

    <html>
    <head>
        <title><?=Title::get()?></title>
    </head>
    <body>...</body>
    </html>


