### Definition of Terms
```
A Hook is a generic term in WordPress that refers to places where you can add your own code or change 
what WordPress is doing or outputting by default. 
Two types of hooks exist in WordPress: actions and filters.
```

### Two Types of Hooks are available
```
1. Action Hook => do_actions(); add_action();
2. Filter Hook => apply_filters(); add_filter();
```

### Action Hook
```
An Action in WordPress is a hook that is triggered at specific time when WordPress is running and 
lets you take an action. This can include things like creating a widget when WordPress is 
initializing or sending a Tweet when someone publishes a post.
```
```
add_action( $hook, $function_to_add, $priority, $accepted_args );
```

### Filter Hook
```
A Filter in WordPress allows you get and modify WordPress data before it is sent to the database 
or the browser. Some examples of filters would include customizing how excerpts are displayed or 
adding some custom code to the end of a blog post.
```
```
add_filter( $tag, $function_to_add, $priority, $accepted_args );
```

#### How to Unhook from Actions and Filters
```
remove_action( $tag, $function_to_remove, $priority );
```
```
remove_filter( $tag, $function_to_remove, $priority );
```

