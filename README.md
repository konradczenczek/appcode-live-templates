# appcode-live-templates
Collection of live templates for AppCode

### wself
Insert weak reference to self.
```
__weak typeof(self) weakSelf = self;
```

### after
Insert dispatch after code block.
```
dispatch_after(dispatch_time(DISPATCH_TIME_NOW, $TIME$ * NSEC_PER_SEC), dispatch_get_main_queue(), ^{
  $CODE$;
});
```

### dtime
Insert dispatch time code block.
```
dispatch_time(DISPATCH_TIME_NOW, $SECONDS$ * NSEC_PER_SEC)
```

### dmain
Insert dispatch async on main queue block.
```
dispatch_async(dispatch_get_main_queue(), ^{
  $END$
})
```

### propns
Insert nonatomic strong property.
```
@property(nonatomic, strong) $DECLARATION$;$END$
```

### propnw
Insert nonatomic weak property.
```
@property(nonatomic, weak) $DECLARATION$;$END$
```

### privcat
Insert private category code block.
```
@interface $CLASS_NAME$ ()
$END$
@end
```

## Installation
Clone this repository in ```~/Library/Preferences/<product><version>/templates``` and restart AppCode.

