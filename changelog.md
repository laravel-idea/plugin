Version 3.3:

* Database factories states and fields completions
* Module system for Laravel package developers
* **Eloquent Helper Code Generation** report
* **Dusk** Test, Page and Component code generations
* Using of `composer.json` PSR-4 namespaces for tests and other non-application classes
* All personal options moved to `.idea/laravel-idea-personal.xml` file. `.idea/laravel-idea.xml` can be pushed to git
* Validation rules completion for `LivewireComponent::rules` and `CompositeRule::rules` methods
* Aliases for main Laravel facades: `class_alias(Illuminate\Support\Facades\Route::class, 'Route')`
* `PDF::loadView` views completion
* Fixes

Version 3.2:

* View, component and livewire component blade variables completion
* Eloquent helper code generation: fetching tables and columns from database + understanding field casts
* Policies completion for `authorize()` and other calls
* New code generation: Optimize Route completions
* Convenient navigation between models and policies (Hot key: **Ctrl-Alt-Home** or **^⌘Up**)
* New module system for modules with own `composer.json` files
* `Blade::component` calls fetching
* Blade `$loop` variable members completion
* Fixes

Version 3.1:

* **Livewire** support + new **Create Livewire Component** code generation
* **nWidart/laravel-modules** package support
* Convenient navigation between events and listeners (Hot key: **Ctrl-Alt-Home** or **^⌘Up**)
* "Add Eloquent model fields" to validation rules array by **Alt-Insert** or **Command(Ctrl)-N**
* Ignore `deleted_at` Eloquent field in some generations
* Fixes

Version 3.0:

* New experimental Eloquent helper code generation! Check **Generate Eloquent Helper Code** code generation
* **Create Blade Component** code generation for Laravel 7 components
* Completion for Blade components from packages
* Nested resource route names support
* Multiple User class support for applications with several Authenticatable classes (comma separated User class setting)
* **Create Module** code generation for module applications
* Fixes

Version 2.4:

* `Route::resources/apiResources` calls route names collecting
* Correct Eloquent relations calls completion. `$this->hasMany(SomeModel::class)->where([SomeModel fields here])`
* New Laravel 7.6 `withoutMiddleware` method parameters completion
* Deprecated controllers and methods are marked as deprecated in route files
* New option "Allow app root module in code generation dialogs" for Directory module system
* Eloquent calculated properties(like `getFirstNameAttribute()` -> `first_name`) completion added
* 'mix' method completion now understands several `mix-manifest.json` files
* Default base class for unit tests is **PHPUnit\Framework\TestCase**
* Fixes

Version 2.3:

* Laravel 7 blade tag components support(to fix Vue errors, please update your IDE to 2020.1 version)
* Artisan commands completion in `$schedule->command()`
* `Log::channel()` completions
* **${DATE} ${TIME} ${YEAR} ${MONTH} ${DAY} ${HOUR} ${MINUTE} ${SECOND}** parameters to file templates
* Eloquent $appends property and append method fields completion
* 'auth:guard_name' middleware completions
* Fixes

Version 2.2:
* **spatie/blade-x** support improvements: recursive directory scanner and inspections suppressor
* `factory()->create()` auto type hinting
* `factory()->create([fields completion])`
* "can:%gate_name%" middleware completions
* `bigIncrements()` instead of `increments()` in migration template
* `Route::is([completion])`
* Fixes

Version 2.1:

* **spatie/blade-x** package support(tags, attributes completion, :attr="%php code injection%")
* `Route::get()->uses([completion])`
* Eloquent `$dispatchesEvents` completion and morph relation methods, like `whereHasMorph()`, support
* Fix registration in "Create Middleware", "Create Listener" and some other generations
* Fix creation translation string from blade - select string and Alt-Ins(or Command(Ctrl)-N)

Version 2.0:

* **Lumen** support
* Create translation keys right from code (**Alt-Insert** or **Command(Ctrl)-N** on PHP string or selected Blade code)
* **Create View Composer** code generation
* `Request::boolean()` method support (added in Laravel 6.12)
* Name parameter of "Create Middleware" become optional
* Model parameter of "Create Json Resource" become optional
* Eloquent `when` method support