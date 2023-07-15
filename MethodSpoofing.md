```php
<form method="post" action="{{route('profile.avatar')}}">
  @method('PATCH') //HTMl does not provide patch request. We need to perform method spoofing.
    <div>
      <x-input-label for="name" value="Avatar" />
      <x-text-input id="avatar" name="avatar" type="file" class="mt-1 block w-full" :value="old('avatar', $user->avatar)" required autofocus autocomplete="avatar" />
      <x-input-error class="mt-2" :messages="$errors->get('avatar')" />
    </div>

    <div class="flex items-center gap-4">
      <x-primary-button>{{ __('Save') }}</x-primary-button>
    </div>
</form>
```

> Equivalent way.

```html
<input type="hidden" name="_method" value="patch" />
```