# appcode-live-templates
Collection on live templates for AppCode

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

### propns
Insert nonatomic strong property.
```
@property(nonatomic, strong) $DECLARATION$;$END$
```

### privcat
Insert private category code block.
```
@interface $CLASS_NAME$ ()
$END$
@end
```

## Installation
TODO

