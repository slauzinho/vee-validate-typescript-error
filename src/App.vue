<template>
  <Form @submit="handleSubmit">
    <Field as="input" label="Name" name="firstname" />
    <button type="submit">Submit</button>
  </Form>
</template>

<script setup lang="ts">
import { Form, Field } from 'vee-validate';

const handleSubmit = (data: { name: string }) => {
  console.log(data);
};
</script>
